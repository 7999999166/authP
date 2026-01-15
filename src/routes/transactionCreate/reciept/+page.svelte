<script>
  // Receipt Against Invoice Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold text-primary-custom mb-4">
      Receipt Against Invoice Form
    </h1>
  </header>

  <main class="flex-grow-1">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 mb-4 rounded bg-transparent">
      <div class="d-flex justify-content-end mb-3">
        <small class="text-secondary">Press ENTER to move forward</small>
      </div>

      <div class="row g-4">
        <div class="col-md-6">
          <div class="d-flex flex-column gap-3">
            <!-- Receipt No -->
            <div class="row align-items-center">
              <label
                for="receipt-no"
                class="col-4 col-form-label text-secondary fw-medium"
                >Receipt No</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control"
                  id="receipt-no"
                  value="Auto Generated"
                  readonly
                />
              </div>
            </div>

            <!-- Voucher Date -->
            <div class="row align-items-center">
              <label
                for="voucher-date"
                class="col-4 col-form-label text-secondary fw-medium"
                >Voucher Date</label
              >
              <div class="col-8 position-relative">
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

        <div class="col-md-6">
          <div class="d-flex flex-column gap-3">
            <!-- Received into -->
            <div class="row align-items-start">
              <label
                for="received-into"
                class="col-4 col-form-label text-secondary fw-medium pt-2"
                >Received into</label
              >
              <div class="col-8">
                <input type="text" class="form-control" id="received-into" />
                <small class="text-secondary d-block mt-1">balance</small>
              </div>
            </div>

            <!-- Received From -->
            <div class="row align-items-start">
              <label
                for="received-from"
                class="col-4 col-form-label text-secondary fw-medium pt-2"
                >Received From</label
              >
              <div class="col-8">
                <input type="text" class="form-control" id="received-from" />
                <small class="text-secondary d-block mt-1">balance</small>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Bottom Section -->
    <div class="border border-secondary-subtle p-4 mb-4 rounded bg-transparent">
      <div class="d-flex justify-content-between align-items-end mb-4">
        <button class="btn btn-light border text-secondary fw-medium">
          Receipt against invoice
        </button>
        <div class="d-flex align-items-center gap-2">
          <label for="amount" class="fw-medium text-secondary text-nowrap"
            >Amount</label
          >
          <input
            type="text"
            class="form-control text-end"
            id="amount"
            value="0"
            style="width: 150px;"
          />
        </div>
      </div>

      <div class="row g-4">
        <div class="col-md-6">
          <div class="d-flex flex-column gap-3">
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="discount" />
              <label
                class="form-check-label fw-medium text-secondary"
                for="discount">Discount</label
              >
            </div>
            <div class="form-check">
              <input
                class="form-check-input"
                type="checkbox"
                id="tax-deducted"
              />
              <label
                class="form-check-label fw-medium text-secondary"
                for="tax-deducted">Tax Deducted</label
              >
            </div>
            <div>
              <label for="narration" class="form-label fw-medium text-secondary"
                >Narration</label
              >
              <textarea class="form-control" id="narration" rows="4"></textarea>
              <small class="text-secondary d-block mt-1"
                >Ctrl+Enter for next line</small
              >
            </div>
          </div>
        </div>

        <div class="col-md-6 d-flex align-items-end justify-content-end">
          <div class="d-flex align-items-center gap-2">
            <label for="total-amount" class="fw-bold text-secondary text-nowrap"
              >Total Amount</label
            >
            <input
              type="text"
              class="form-control text-end fw-bold"
              id="total-amount"
              value="0.00"
              style="width: 150px;"
            />
          </div>
        </div>
      </div>
    </div>
  </main>

  <!-- Footer -->
  <footer
    class="mt-4 pt-4 border-top border-secondary-subtle d-flex justify-content-between align-items-center"
  >
    <button class="btn btn-light border text-secondary fw-medium">
      Ctrl+Q: Exit
    </button>
    <button class="btn btn-primary-action text-white fw-medium">
      F12:Save
    </button>
  </footer>
</div>

<style>
  /* Custom colors for this page to match original exactly */
  :global(:root) {
    --primary-custom: #1d3557;
    --primary-action: #03045e;
  }

  .text-primary-custom {
    color: var(--primary-custom);
  }

  .btn-primary-action {
    background-color: var(--primary-action);
    border-color: var(--primary-action);
  }

  .btn-primary-action:hover {
    background-color: #020344;
    border-color: #020344;
  }

  .bg-background-light {
    background-color: var(--background-light);
  }

  .form-control,
  .form-select {
    padding: 0.5rem 0.75rem;
  }
</style>
