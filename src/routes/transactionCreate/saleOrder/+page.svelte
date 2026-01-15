<script>
  // Sale Order Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: #03045e;">Sale Order Form</h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <div class="col-md-6">
          <div class="d-flex flex-column gap-3">
            <div class="row align-items-center">
              <label
                for="estimate-no"
                class="col-4 col-form-label text-secondary fw-medium text-end"
                >Sale Order No</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control bg-white"
                  id="estimate-no"
                  value="Auto Generated"
                  readonly
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="record-date"
                class="col-4 col-form-label text-secondary fw-medium text-end"
                >Record Date</label
              >
              <div class="col-8 position-relative">
                <input
                  type="text"
                  class="form-control"
                  id="record-date"
                  value="16 November 2025"
                />
                <span
                  class="position-absolute top-50 end-0 translate-middle-y me-3 text-secondary"
                >
                  <i class="bi bi-calendar"></i>
                </span>
              </div>
            </div>
          </div>
        </div>

        <div class="col-md-6">
          <div class="d-flex flex-column gap-3">
            <div class="row align-items-start">
              <label
                for="customer"
                class="col-4 col-form-label text-secondary fw-medium text-end pt-2"
                >Customer/Debtor</label
              >
              <div class="col-8">
                <input type="text" class="form-control" id="customer" />
                <small class="text-secondary d-block mt-1">balance</small>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Item Entry & Table Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4 mb-3">
        <div class="col-md-6">
          <label for="f9-item" class="fw-medium text-secondary mb-1"
            >F9: Inventory Item</label
          >
          <input type="text" class="form-control" id="f9-item" />
          <small class="text-secondary d-block mt-1"
            >Press ENTER key to add item.</small
          >
        </div>
        <div class="col-md-6">
          <label for="f10-service" class="fw-medium text-secondary mb-1"
            >F10: Service</label
          >
          <input type="text" class="form-control" id="f10-service" />
        </div>
      </div>

      <div class="d-flex justify-content-between align-items-center mb-3 small">
        <div class="d-flex gap-3">
          <span class="text-secondary"
            >Units Left: <span class="text-primary fw-medium">0</span></span
          >
          <a href="#" class="text-primary text-decoration-none"
            >Alt+F2: Item History</a
          >
          <a href="#" class="text-primary text-decoration-none">View Photo</a>
        </div>
        <small class="text-secondary"
          >Press DELETE key to remove item row.</small
        >
      </div>

      <div class="table-responsive border border-secondary-subtle rounded mb-3">
        <table class="table table-hover mb-0">
          <thead class="table-light">
            <tr>
              <th class="small text-secondary text-uppercase fw-medium">Item</th
              >
              <th
                class="small text-secondary text-uppercase fw-medium"
                style="width: 100px;">QTY</th
              >
              <th
                class="small text-secondary text-uppercase fw-medium"
                style="width: 120px;">Rate</th
              >
              <th
                class="small text-secondary text-uppercase fw-medium"
                style="width: 120px;">Value</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Description</th
              >
            </tr>
          </thead>
          <tbody>
            <tr>
              <td colspan="5" class="text-center text-secondary py-5"></td>
            </tr>
          </tbody>
        </table>
      </div>

      <div class="d-flex justify-content-end align-items-center gap-2">
        <label for="amount" class="fw-medium text-secondary">Amount</label>
        <input
          type="text"
          class="form-control bg-light text-end fw-semibold"
          id="amount"
          value="0"
          readonly
          style="width: 130px;"
        />
      </div>
    </div>

    <!-- Bottom Section -->
    <div class="row g-4">
      <!-- Left Column -->
      <div class="col-md-6">
        <div class="d-flex flex-column gap-3">
          <div class="d-flex gap-4">
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="discount" />
              <label
                class="form-check-label text-secondary fw-medium"
                for="discount">Discount %</label
              >
            </div>
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="tax-check" />
              <label
                class="form-check-label text-secondary fw-medium"
                for="tax-check">Tax</label
              >
            </div>
          </div>

          <div>
            <label for="narration" class="fw-medium text-secondary mb-1"
              >Narration</label
            >
            <textarea class="form-control" id="narration" rows="3"></textarea>
            <small class="text-secondary d-block mt-1"
              >Ctrl+Enter for next line</small
            >
          </div>

          <div>
            <label for="terms" class="fw-medium text-secondary mb-1"
              >Terms Conditions</label
            >
            <textarea class="form-control" id="terms" rows="2"></textarea>
          </div>
        </div>
      </div>

      <!-- Right Column -->
      <div
        class="col-md-6 d-flex flex-column justify-content-between align-items-end"
      >
        <div class="w-100 d-flex flex-column gap-3" style="max-width: 300px;">
          <div class="d-flex justify-content-end align-items-center gap-2">
            <label for="round-off" class="fw-medium text-secondary"
              >Round Off</label
            >
            <input
              type="text"
              class="form-control text-end"
              id="round-off"
              style="width: 130px;"
            />
          </div>
          <div class="d-flex justify-content-end align-items-center gap-2">
            <label for="total-amount" class="fw-medium text-secondary"
              >Total Amount</label
            >
            <input
              type="text"
              class="form-control bg-light text-end fw-semibold"
              id="total-amount"
              value="0"
              readonly
              style="width: 130px;"
            />
          </div>
        </div>

        <div
          class="border border-secondary-subtle p-3 rounded mt-3 w-100"
          style="max-width: 300px;"
        >
          <label class="fw-medium text-secondary d-block mb-2">Tax</label>
          <div class="d-flex flex-column gap-2">
            <div class="form-check">
              <input
                class="form-check-input"
                type="radio"
                name="tax-option"
                id="tax-total"
                checked
              />
              <label class="form-check-label text-secondary" for="tax-total"
                >On Total</label
              >
            </div>
            <div class="form-check">
              <input
                class="form-check-input"
                type="radio"
                name="tax-option"
                id="tax-item"
              />
              <label class="form-check-label text-secondary" for="tax-item"
                >Per Item</label
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>

  <!-- Footer -->
  <footer
    class="mt-4 pt-4 border-top border-secondary-subtle d-flex justify-content-between align-items-center sticky-bottom bg-background-light z-1 p-3 mx-n4 mb-n4"
  >
    <button class="btn btn-light border text-secondary fw-medium">
      Ctrl+Q: Exit
    </button>
    <div class="d-flex gap-2">
      <button class="btn btn-light border text-secondary fw-medium">
        Alt+F12: Save & View
      </button>
      <button class="btn btn-primary fw-medium"> F12:Save </button>
    </div>
  </footer>
</div>

<style>
  .bg-background-light {
    background-color: var(--background-light);
  }
  .form-control,
  .form-select {
    padding: 0.5rem 0.75rem;
  }
</style>
