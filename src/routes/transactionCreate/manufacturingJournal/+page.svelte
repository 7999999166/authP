<script>
  // Manufacturing Journal Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: #03045e;">
      Manufacturing Journal Form
    </h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <div class="col-md-6">
          <div class="d-flex flex-column gap-3">
            <div class="row align-items-center">
              <label
                for="manufacturing-template"
                class="col-4 col-form-label text-secondary fw-medium"
                >Manufacturing Template</label
              >
              <div class="col-8">
                <select class="form-select" id="manufacturing-template">
                  <option></option>
                </select>
              </div>
            </div>

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

            <div class="row align-items-center">
              <label
                for="voucher-no"
                class="col-4 col-form-label text-secondary fw-medium"
                >Voucher No</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control bg-white"
                  id="voucher-no"
                  value="Auto Generated"
                  readonly
                />
              </div>
            </div>
          </div>
        </div>
      </div>
      <small class="text-secondary d-block mt-3"
        >Press ENTER to move forward & SHIFT+ENTER to move back.</small
      >
    </div>

    <!-- Tables Section -->
    <div class="row g-4">
      <!-- Consumed Items -->
      <div class="col-lg-6">
        <div
          class="border border-secondary-subtle p-4 rounded bg-transparent h-100"
        >
          <div class="d-flex justify-content-between align-items-center mb-3">
            <div class="d-flex align-items-center gap-2">
              <label for="consumed-item-input" class="fw-medium text-secondary"
                >F9: Consumed Items</label
              >
              <input
                type="text"
                class="form-control"
                id="consumed-item-input"
                style="width: 200px;"
              />
            </div>
            <a href="#" class="text-primary text-decoration-none small"
              >Alt+F1: Warehouse</a
            >
          </div>

          <div class="table-responsive border border-secondary-subtle rounded">
            <table class="table table-hover mb-0">
              <thead class="table-light">
                <tr>
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Item</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Warehouse</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Quantity</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Rate/Unit</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Amount</th
                  >
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td colspan="5" class="text-center text-secondary py-5">
                    No items added.
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>

      <!-- Manufactured Items -->
      <div class="col-lg-6">
        <div
          class="border border-secondary-subtle p-4 rounded bg-transparent h-100"
        >
          <div class="d-flex justify-content-between align-items-center mb-3">
            <div class="d-flex align-items-center gap-2">
              <label
                for="manufactured-item-input"
                class="fw-medium text-secondary">F10: Manufactured Items</label
              >
              <input
                type="text"
                class="form-control"
                id="manufactured-item-input"
                style="width: 200px;"
              />
            </div>
            <a href="#" class="text-primary text-decoration-none small"
              >Alt+F1: Warehouse Units</a
            >
          </div>

          <div class="table-responsive border border-secondary-subtle rounded">
            <table class="table table-hover mb-0">
              <thead class="table-light">
                <tr>
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Item</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Warehouse</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Quantity</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Rate/Unit</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >% of Total</th
                  >
                  <th class="small text-secondary text-uppercase fw-medium"
                    >Amount</th
                  >
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td colspan="6" class="text-center text-secondary py-5">
                    No items added.
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>

    <!-- Bottom Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <div class="col-lg-4">
          <div class="d-flex flex-column gap-3">
            <div class="row align-items-center">
              <label
                for="cost-components"
                class="col-6 col-form-label text-secondary fw-medium"
                >Cost of Components</label
              >
              <div class="col-6">
                <input
                  type="text"
                  class="form-control bg-light text-center fw-semibold"
                  id="cost-components"
                  value="0.00"
                  readonly
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="manufacturing-expense"
                class="col-6 col-form-label text-secondary fw-medium"
                >Manufacturing Expense</label
              >
              <div class="col-6">
                <input
                  type="text"
                  class="form-control text-end"
                  id="manufacturing-expense"
                  value="0.00"
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="total-value"
                class="col-6 col-form-label text-secondary fw-medium"
                >Total Value</label
              >
              <div class="col-6">
                <input
                  type="text"
                  class="form-control bg-light text-center fw-semibold"
                  id="total-value"
                  value="0.00"
                  readonly
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="balance-amount"
                class="col-6 col-form-label text-secondary fw-medium"
                >Balance Amount</label
              >
              <div class="col-6">
                <input
                  type="text"
                  class="form-control bg-light text-center fw-semibold"
                  id="balance-amount"
                  value="0.00"
                  readonly
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="balance-percentage"
                class="col-6 col-form-label text-secondary fw-medium"
                >Balance Percentage</label
              >
              <div class="col-6">
                <input
                  type="text"
                  class="form-control bg-light text-center fw-semibold"
                  id="balance-percentage"
                  value="100.00"
                  readonly
                />
              </div>
            </div>
          </div>
        </div>

        <div class="col-lg-8">
          <div class="d-flex flex-column gap-3">
            <div>
              <label for="narration" class="fw-medium text-secondary mb-1"
                >Narration</label
              >
              <textarea class="form-control" id="narration" rows="5"></textarea>
              <small class="text-secondary d-block mt-1"
                >Ctrl+Enter for next line</small
              >
            </div>

            <div class="d-flex align-items-center gap-3">
              <div class="d-flex align-items-center gap-2">
                <label for="multiplier" class="fw-medium text-secondary"
                  >Multiplier</label
                >
                <input
                  type="text"
                  class="form-control"
                  id="multiplier"
                  value="1"
                  style="width: 80px;"
                />
                <button class="btn btn-light border text-secondary fw-medium"
                  >Calculate</button
                >
              </div>
              <small class="text-secondary"
                >Note: Manufacturing Expense won't effect account balances. You
                need to create a separate Expense transaction.</small
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
    <div class="d-flex gap-2">
      <button class="btn btn-light border text-secondary fw-medium">
        Ctrl+Q: Exit
      </button>
      <a
        href="#"
        class="btn btn-light border text-secondary fw-medium text-decoration-none"
      >
        Video: How to Manufacturing Journal?
      </a>
    </div>
    <div class="d-flex gap-2">
      <button class="btn btn-light border text-secondary fw-medium">
        Save Template
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
