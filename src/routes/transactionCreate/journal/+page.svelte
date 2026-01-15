<script>
  // Journal Entry Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: #03045e;">Journal Entry Form</h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <small class="text-secondary d-block mb-3"
        >Press ENTER to move forward & SHIFT+ENTER to move back.</small
      >

      <div class="row g-4">
        <div class="col-lg-4 col-md-6">
          <div class="d-flex flex-column gap-2">
            <label for="journal-no" class="fw-medium text-secondary"
              >Journal No</label
            >
            <input
              type="text"
              class="form-control bg-white"
              id="journal-no"
              value="Auto Generated"
              readonly
            />
          </div>
        </div>

        <div class="col-lg-4 col-md-6">
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

        <div class="col-lg-4 col-md-6">
          <div class="d-flex flex-column gap-2">
            <label for="default" class="fw-medium text-secondary">Default</label
            >
            <input
              type="text"
              class="form-control"
              id="default"
              value="DEFAULT"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- Account Selection -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row">
        <div class="col-md-6">
          <label for="select-account" class="fw-medium text-secondary mb-2"
            >F9: Select Account</label
          >
          <input type="text" class="form-control" id="select-account" />
          <div class="d-flex justify-content-between mt-1">
            <small class="text-secondary">Press ENTER key to add.</small>
            <a href="#" class="text-primary text-decoration-none small"
              >balance</a
            >
          </div>
        </div>
      </div>
    </div>

    <!-- Table Section -->
    <div class="border border-secondary-subtle rounded overflow-hidden">
      <div class="table-responsive">
        <table class="table table-hover mb-0">
          <thead class="table-light">
            <tr>
              <th class="small text-secondary text-uppercase fw-medium"
                >Account</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Debit Amount</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Credit Amount</th
              >
            </tr>
          </thead>
          <tbody>
            <tr>
              <td colspan="3" class="text-center text-secondary py-5">
                No entries added.
              </td>
            </tr>
          </tbody>
        </table>
      </div>

      <div
        class="d-flex justify-content-end align-items-center gap-4 p-3 bg-light border-top border-secondary-subtle"
      >
        <div class="d-flex align-items-center gap-2">
          <label for="debit-total" class="fw-medium text-secondary"
            >Debit Total</label
          >
          <input
            type="text"
            class="form-control bg-light text-center fw-semibold"
            id="debit-total"
            value="0.00"
            readonly
            style="width: 150px;"
          />
        </div>
        <div class="d-flex align-items-center gap-2">
          <label for="credit-total" class="fw-medium text-secondary"
            >Credit Total</label
          >
          <input
            type="text"
            class="form-control bg-light text-center fw-semibold"
            id="credit-total"
            value="0"
            readonly
            style="width: 150px;"
          />
        </div>
      </div>
    </div>

    <!-- Narration -->
    <div>
      <label for="narration" class="fw-medium text-secondary mb-2"
        >Narration</label
      >
      <textarea class="form-control" id="narration" rows="3"></textarea>
      <small class="text-secondary d-block mt-1"
        >Use Ctrl+Enter for next line</small
      >
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
      <button class="btn btn-light border text-secondary fw-medium p-2">
        <i class="bi bi-calculator"></i>
      </button>
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
