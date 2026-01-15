<script>
  // Payment Entry Form (Expense)
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: #023047;">Payment Entry Form</h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <small class="text-secondary d-block mb-3"
        >Press ENTER to move forward & SHIFT+ENTER to move back.</small
      >

      <div class="row g-4">
        <div class="col-md-4">
          <div class="d-flex flex-column gap-3">
            <div class="d-flex flex-column gap-2">
              <label for="payment-no" class="fw-medium text-secondary"
                >Payment No</label
              >
              <input
                type="text"
                class="form-control bg-light"
                id="payment-no"
                value="Auto Generated"
                readonly
              />
            </div>

            <div class="d-flex flex-column gap-2">
              <label for="voucher-date" class="fw-medium text-secondary"
                >Voucher Date</label
              >
              <div class="position-relative">
                <input
                  type="text"
                  class="form-control"
                  id="voucher-date"
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

        <div class="col-md-4"></div>

        <div class="col-md-4">
          <div class="d-flex flex-column gap-3">
            <div class="d-flex flex-column gap-2">
              <label for="paid-from" class="fw-medium text-secondary"
                >Paid From</label
              >
              <input type="text" class="form-control" id="paid-from" />
              <small class="text-primary">balance</small>
            </div>

            <div class="d-flex flex-column gap-2">
              <label for="paid-to" class="fw-medium text-secondary"
                >F9: Paid To</label
              >
              <input type="text" class="form-control" id="paid-to" />
              <small class="text-primary">balance</small>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Table Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <p class="small fw-medium text-primary mb-2">Press ENTER key to add.</p>

      <div class="table-responsive border border-secondary-subtle rounded">
        <table class="table table-hover mb-0">
          <thead class="table-light">
            <tr>
              <th class="small text-secondary text-uppercase fw-medium"
                >Account</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Amount</th
              >
            </tr>
          </thead>
          <tbody>
            <tr>
              <td colspan="2" class="text-center text-secondary py-5">
                No entries added.
              </td>
            </tr>
          </tbody>
        </table>
      </div>

      <div class="d-flex justify-content-end align-items-center mt-3 gap-3">
        <label for="total" class="fw-bold text-secondary">Total</label>
        <input
          type="text"
          class="form-control bg-light text-end fw-semibold"
          id="total"
          value="0.00"
          readonly
          style="width: 150px;"
        />
      </div>
    </div>

    <!-- Narration -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="d-flex flex-column gap-2">
        <label for="narration" class="fw-medium text-secondary">Narration</label
        >
        <textarea class="form-control" id="narration" rows="3"></textarea>
        <small class="text-secondary">Use Ctrl+Enter for next line</small>
      </div>
    </div>
  </main>

  <!-- Footer -->
  <footer
    class="mt-4 pt-4 border-top border-secondary-subtle d-flex justify-content-between align-items-center sticky-bottom bg-background-light z-1 p-3 mx-n4 mb-n4"
  >
    <div>
      <button class="btn btn-light border text-secondary fw-medium">
        Ctrl+Q: Exit
      </button>
    </div>
    <div class="d-flex gap-2">
      <button class="btn btn-light border text-secondary fw-medium p-2">
        <i class="bi bi-calculator"></i>
      </button>
      <button class="btn btn-light border text-secondary fw-medium">
        Alt+F12: Save & View
      </button>
      <button class="btn btn-primary fw-medium"> F12: Save </button>
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
