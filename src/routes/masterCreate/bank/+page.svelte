<script>
  import { onMount } from "svelte";
  import { page } from "$app/stores";

  let accessToken = $state("");

  onMount(() => {
    const searchParams = $page.url.searchParams;
    accessToken = searchParams.get("access_token") || "";
    console.log("Access Token:", accessToken);
    handleGoogleResponse(accessToken);

  });

  async function handleGoogleResponse(response) {
    const idToken = response; 

    const res = await fetch(
      "https://strapifebs-production.up.railway.app/api/connect/google/callback",
      {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({ id_token: idToken }),
      },
    );

    const data = await res.json();
    const { jwt, user } = data;
    localStorage.setItem("jwt", jwt);
    console.log("Logged in user:", user);
  }

</script>

<div class="container-fluid p-4">
  <div class="shadow-sm p-3 rounded-4">
    <div class="card-header border-bottom py-3">
      <div class="d-flex justify-content-between align-items-center">
        <h5 class="mb-0 fw-bold">Create Bank Accounts</h5>
      </div>
    </div>
    <div class="card-body">
      <form>
        <div class="row g-3 pt-3">
          <!-- Left Column -->
          <div class="col-md-6">
            <div class="mb-3">
              <label for="account-type" class="form-label fw-bold"
                >Account Type</label
              >
              <input
                type="text"
                class="form-control"
                id="account-type"
                placeholder="e.g. Savings"
                required
              />
            </div>
            <div class="mb-3">
              <label for="account-name" class="form-label fw-bold"
                >Account Name</label
              >
              <input
                type="text"
                class="form-control"
                id="account-name"
                placeholder="e.g. Primary Account"
                required
              />
            </div>
            <div class="mb-3">
              <label for="account-group" class="form-label fw-bold"
                >Account Group</label
              >
              <input
                type="text"
                class="form-control"
                id="account-group"
                placeholder="e.g. Personal"
              />
            </div>
            <div class="mb-3">
              <label for="creation-date" class="form-label fw-bold"
                >Account Creation Date</label
              >
              <input
                type="date"
                class="form-control"
                id="creation-date"
                required
              />
            </div>
            <div class="mb-3">
              <label for="opening-balance" class="form-label fw-bold"
                >Opening Balance</label
              >
              <input
                type="number"
                class="form-control"
                id="opening-balance"
                placeholder="0.00"
                min="0"
                step="0.01"
                required
              />
            </div>
          </div>

          <!-- Right Column -->
          <div class="col-md-6">
            <div class="mb-3">
              <label for="bank-account-holder" class="form-label fw-bold"
                >Bank Account Holder</label
              >
              <input
                type="text"
                class="form-control"
                id="bank-account-holder"
                placeholder="e.g. John Doe"
              />
            </div>
            <div class="mb-3">
              <label for="bank-name-branch" class="form-label fw-bold"
                >Bank Name and Branch</label
              >
              <input
                type="text"
                class="form-control"
                id="bank-name-branch"
                placeholder="e.g. Central Bank, Downtown Branch"
              />
            </div>
            <div class="mb-3">
              <label for="account-number" class="form-label fw-bold"
                >Account Number</label
              >
              <input
                type="text"
                class="form-control"
                id="account-number"
                placeholder="Enter account number"
                pattern="[0-9]{(9, 18)}"
              />
            </div>
          </div>

          <!-- Full Width -->
          <div class="col-12 mt-3">
            <label for="remarks" class="form-label fw-bold">Remarks</label>
            <textarea
              class="form-control"
              id="remarks"
              rows="4"
              placeholder="Add any relevant notes here..."
            ></textarea>
          </div>

          <div class="col-12 text-end mt-4 sticky-bottom">
            <button
              type="submit"
              class="btn btn-primary px-4 fw-bold"
              style="background-color: #03045e; border-color: #03045e;"
              >Save Changes</button
            >
          </div>
        </div>
      </form>
    </div>
  </div>
</div>
