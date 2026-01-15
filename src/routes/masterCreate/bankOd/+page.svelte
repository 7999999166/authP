<script>

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
          <!-- Right Column -->
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
          </div>

          <!-- Left Column -->
          <div class="col-md-6">
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
