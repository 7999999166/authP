<script>
  // Purchase Entry Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: #03045e;">Purchase Entry Form</h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <!-- Row 1 -->
        <div class="col-md-3">
          <div class="d-flex flex-column gap-2">
            <label for="purchase-no" class="fw-medium text-secondary"
              >Purchase No</label
            >
            <input
              type="text"
              class="form-control bg-white"
              id="purchase-no"
              value="Auto Generated"
              readonly
            />
          </div>
        </div>
        <div class="col-md-3">
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
        <div class="col-md-3">
          <div class="d-flex flex-column gap-2">
            <label for="supplier-invoice-no" class="fw-medium text-secondary"
              >Supplier Invoice No.</label
            >
            <input type="text" class="form-control" id="supplier-invoice-no" />
          </div>
        </div>
        <div class="col-md-3">
          <div class="d-flex flex-column gap-2">
            <label for="place-of-supply" class="fw-medium text-secondary"
              >Place Of Supply</label
            >
            <select class="form-select" id="place-of-supply">
              <option>Delhi</option>
            </select>
          </div>
        </div>

        <!-- Row 2 -->
        <div class="col-md-6">
          <div class="d-flex flex-column gap-2">
            <label for="purchase-account" class="fw-medium text-secondary"
              >Purchase Account</label
            >
            <input
              type="text"
              class="form-control"
              id="purchase-account"
              value="Purchase"
            />
          </div>
        </div>
        <div class="col-md-6">
          <div class="d-flex flex-column gap-2">
            <label for="supplier-cash" class="fw-medium text-secondary"
              >Supplier/Cash</label
            >
            <input type="text" class="form-control" id="supplier-cash" />
            <small class="text-secondary">balance</small>
          </div>
        </div>

        <!-- Row 3 -->
        <div class="col-md-6">
          <div class="d-flex align-items-center gap-4 h-100 pt-3">
            <div class="d-flex align-items-center gap-2">
              <i class="bi bi-geo-alt-fill text-danger"></i>
              <div class="form-check mb-0">
                <input
                  class="form-check-input"
                  type="radio"
                  name="location"
                  id="local"
                  checked
                />
                <label
                  class="form-check-label text-secondary fw-medium"
                  for="local">Local</label
                >
              </div>
            </div>
            <div class="form-check mb-0">
              <input
                class="form-check-input"
                type="radio"
                name="location"
                id="interstate"
              />
              <label
                class="form-check-label text-secondary fw-medium"
                for="interstate">Interstate</label
              >
            </div>
            <input
              type="text"
              class="form-control"
              value="DEFAULT"
              style="width: 120px;"
            />
          </div>
        </div>
        <div class="col-md-6">
          <div class="d-flex flex-column gap-2">
            <label for="due-date" class="fw-medium text-secondary"
              >Due Date</label
            >
            <div class="position-relative">
              <input
                type="text"
                class="form-control"
                id="due-date"
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
    </div>

    <!-- Item Entry & Table Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="d-flex justify-content-between text-secondary small mb-3">
        <span>Press ENTER to move forward</span>
        <span>DELETE: To Delete Row, Shift+UP/Down: To Rearrange Items</span>
      </div>

      <div class="row g-4 mb-3">
        <div class="col-md-6">
          <div class="d-flex align-items-center gap-2">
            <label for="f9-item" class="fw-medium text-secondary text-nowrap"
              >F9: Item</label
            >
            <input type="text" class="form-control" id="f9-item" />
          </div>
        </div>
        <div class="col-md-6">
          <div class="d-flex align-items-center gap-2">
            <label
              for="f10-service"
              class="fw-medium text-secondary text-nowrap">F10: Service</label
            >
            <input type="text" class="form-control" id="f10-service" />
          </div>
        </div>
      </div>

      <div class="d-flex gap-4 small fw-medium text-primary mb-3">
        <span>Units Left: 0</span>
        <span>Alt+F1: Warehouse</span>
        <span>Alt+F2: Item History</span>
      </div>

      <div class="table-responsive border border-secondary-subtle rounded mb-3">
        <table class="table table-hover mb-0">
          <thead class="table-light">
            <tr>
              <th class="small text-secondary text-uppercase fw-medium">Item</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Warehouse</th
              >
              <th class="small text-secondary text-uppercase fw-medium">QTY</th>
              <th class="small text-secondary text-uppercase fw-medium"
                >Units</th
              >
              <th class="small text-secondary text-uppercase fw-medium">Rate</th
              >
              <th class="small text-secondary text-uppercase fw-medium">Per</th>
              <th class="small text-secondary text-uppercase fw-medium"
                >Value</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Description</th
              >
            </tr>
          </thead>
          <tbody>
            <tr>
              <td colspan="8" class="text-center text-secondary py-5">
                No items added
              </td>
            </tr>
          </tbody>
        </table>
      </div>

      <div class="d-flex justify-content-end align-items-center gap-2">
        <label for="amount" class="fw-medium text-secondary">Amount</label>
        <input
          type="text"
          class="form-control text-end"
          id="amount"
          value="0.00"
          style="width: 150px;"
        />
      </div>
    </div>

    <!-- Bottom Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent mb-5">
      <div class="row g-4">
        <!-- Left Column -->
        <div class="col-md-5">
          <div class="d-flex flex-column gap-3">
            <div class="d-flex flex-column gap-2">
              <div class="form-check">
                <input class="form-check-input" type="checkbox" id="discount" />
                <label
                  class="form-check-label text-secondary fw-medium"
                  for="discount">Discount</label
                >
              </div>
              <div class="form-check">
                <input class="form-check-input" type="checkbox" id="tax" />
                <label
                  class="form-check-label text-secondary fw-medium"
                  for="tax">Tax</label
                >
              </div>
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="checkbox"
                  id="other-charges"
                />
                <label
                  class="form-check-label text-secondary fw-medium"
                  for="other-charges">Other Charges</label
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

            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="dispatch" />
              <label
                class="form-check-label text-secondary fw-medium"
                for="dispatch">Dispatch</label
              >
            </div>
          </div>
        </div>

        <div class="col-md-3"></div>

        <!-- Right Column -->
        <div
          class="col-md-4 d-flex flex-column justify-content-between align-items-end"
        >
          <div class="w-100 d-flex flex-column gap-3" style="max-width: 300px;">
            <div
              class="d-flex justify-content-between align-items-center gap-2"
            >
              <label for="round-off" class="fw-medium text-secondary"
                >Round Off</label
              >
              <input
                type="text"
                class="form-control text-end"
                id="round-off"
                value="0.00"
                style="width: 130px;"
              />
            </div>
            <div
              class="d-flex justify-content-between align-items-center gap-2"
            >
              <label for="total-amount" class="fw-bold text-secondary"
                >Total Amount</label
              >
              <input
                type="text"
                class="form-control text-end fw-bold"
                id="total-amount"
                value="0.00"
                style="width: 130px;"
              />
            </div>
          </div>

          <div
            class="border border-secondary-subtle p-3 rounded mt-3 w-100"
            style="max-width: 300px;"
          >
            <label class="fw-medium text-secondary d-block mb-2"
              >Discount & Tax</label
            >
            <div class="d-flex flex-column gap-2">
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="radio"
                  name="discount-tax"
                  id="on-total"
                  checked
                />
                <label
                  class="form-check-label text-secondary fw-medium"
                  for="on-total">On Total</label
                >
              </div>
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="radio"
                  name="discount-tax"
                  id="per-item"
                />
                <label
                  class="form-check-label text-secondary fw-medium"
                  for="per-item">Per Item</label
                >
              </div>
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
        Ctrl+F12: Save & Payment
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
