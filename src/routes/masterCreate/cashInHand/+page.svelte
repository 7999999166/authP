<script>
  // Master Create: Cash In Hand
  // Converted from page.html
</script>

<div class="container-fluid p-4">
  <div class="card shadow-sm">
    <div class="card-header bg-white border-bottom py-3">
      <div class="d-flex justify-content-between align-items-center">
        <h5 class="mb-0 fw-bold">Account Details</h5>
        <div>
          <button class="btn btn-light btn-sm me-1"
            ><i class="bi bi-bell"></i></button
          >
          <button class="btn btn-light btn-sm"
            ><i class="bi bi-gear"></i></button
          >
        </div>
      </div>
    </div>
    <div class="card-body">
      <form>
        <div class="row g-3">
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

          <div class="col-md-6">
            <!-- Right column in HTML only had GSTIN -->
            <div class="mb-3">
              <label for="gstin" class="form-label fw-bold">GSTIN</label>
              <input
                type="text"
                class="form-control"
                id="gstin"
                placeholder="e.g. 22AAAAA0000A1Z5"
                pattern="[0-9]{2}[A-Z]{5}[0-9]{4}[A-Z]{1}[1-9A-Z]{1}Z[0-9A-Z]{1}"
              />
            </div>
          </div>

          <div class="col-12">
            <label for="remarks" class="form-label fw-bold">Remarks</label>
            <textarea
              class="form-control"
              id="remarks"
              rows="4"
              placeholder="Add any relevant notes here..."
            ></textarea>
          </div>

          <div class="col-12 text-end mt-4">
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
