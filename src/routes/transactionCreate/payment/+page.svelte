<script>
  // Payment Against Purchases Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold text-primary">Payment Against Purchases Form</h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <!-- Payment No -->
        <div class="col-md-6">
          <div class="row align-items-center">
            <label for="payment-no" class="col-4 col-form-label text-secondary fw-medium">Payment No</label>
            <div class="col-8">
              <input
                type="text"
                class="form-control bg-light text-secondary"
                id="payment-no"
                value="Auto Generated"
                readonly
              />
            </div>
          </div>
        </div>

        <!-- Voucher Date -->
        <div class="col-md-6">
          <div class="row align-items-center">
            <label for="voucher-date" class="col-4 col-form-label text-secondary fw-medium">Voucher Date</label>
            <div class="col-8 position-relative">
              <input
                type="text"
                class="form-control"
                id="voucher-date"
                value="16 November 2025"
              />
              <span class="position-absolute top-50 end-0 translate-middle-y me-3 text-secondary">
                <i class="bi bi-calendar"></i>
              </span>
            </div>
          </div>
        </div>

        <!-- Paid To -->
        <div class="col-md-6">
          <div class="row align-items-start">
            <label for="paid-to" class="col-4 col-form-label text-secondary fw-medium pt-2">Paid To</label>
            <div class="col-8">
              <input type="text" class="form-control" id="paid-to" />
              <small class="text-secondary d-block mt-1">balance</small>
            </div>
          </div>
        </div>

        <!-- Paid From -->
        <div class="col-md-6">
          <div class="row align-items-start">
            <label for="paid-from" class="col-4 col-form-label text-secondary fw-medium pt-2">Paid From</label>
            <div class="col-8">
              <input type="text" class="form-control" id="paid-from" />
              <small class="text-secondary d-block mt-1">balance</small>
            </div>
          </div>
        </div>
      </div>

      <!-- Helper Text -->
      <div class="mt-3 text-center">
        <span class="small fw-medium text-secondary">Press ENTER to move forward</span>
      </div>
    </div>

    <!-- Middle Section -->
    <div class="row g-4">
      <!-- Payment Type & Options -->
      <div class="col-md-6">
        <div class="border border-secondary-subtle p-4 rounded bg-transparent h-100">
          <button class="btn btn-light border w-100 text-start fw-medium mb-3">
            Payment against purchases
          </button>

          <div class="d-flex flex-column gap-2">
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="discount" />
              <label class="form-check-label fw-medium text-secondary" for="discount">
                Discount
              </label>
            </div>
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="tax-deducted" />
              <label class="form-check-label fw-medium text-secondary" for="tax-deducted">
                Tax Deducted
              </label>
            </div>
          </div>
        </div>
      </div>

      <!-- Amount -->
      <div class="col-md-6">
        <div class="border border-secondary-subtle p-4 rounded bg-transparent h-100 d-flex flex-column justify-content-center">
          <div class="d-flex align-items-center justify-content-between gap-3">
            <label for="amount" class="fw-medium text-secondary">Amount</label>
            <input
              type="text"
              class="form-control bg-light text-end fw-medium"
              id="amount"
              value="0"
              readonly
              style="width: 200px;"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- Bottom Section -->
    <div class="row g-4">
      <!-- Narration -->
      <div class="col-md-8">
        <div class="d-flex flex-column gap-2">
          <label for="narration" class="fw-medium text-secondary">Narration</label>
          <textarea class="form-control" id="narration" rows="3"></textarea>
          <small class="text-secondary">Ctrl+Enter for next line</small>
        </div>
      </div>

      <!-- Total Amount -->
      <div class="col-md-4 d-flex align-items-end justify-content-end">
        <div class="border border-secondary-subtle p-3 rounded w-100">
          <div class="d-flex align-items-center justify-content-between">
            <label for="total-amount" class="fw-bold text-secondary">Total Amount</label>
            <input
              type="text"
              class="form-control bg-light text-end fw-bold fs-5"
              id="total-amount"
              value="0.00"
              readonly
              style="width: 150px;"
            />
          </div>
        </div>
      </div>
    </div>
  </main>

  <!-- Footer Action Bar -->
  <footer class="mt-5 pt-3 border-top border-secondary-subtle d-flex justify-content-between align-items-center sticky-bottom bg-background-light z-1 p-3 mx-n4 mb-n4">
    <button class="btn btn-light border text-secondary fw-medium">
      Ctrl+Q: Exit
    </button>
    <div class="d-flex gap-2">
      <button class="btn btn-primary d-flex align-items-center gap-1 fw-medium shadow-sm">
        F12: Save
        <i class="bi bi-chevron-right small"></i>
      </button>
    </div>
  </footer>
</div>

<style>
  /* Scoped styles for specific tweaks */
  .bg-background-light {
    background-color: var(--background-light);
  }
  
  /* Ensure inputs match the design height/padding */
  .form-control, .form-select {
    padding: 0.5rem 0.75rem;
  }
</style>
