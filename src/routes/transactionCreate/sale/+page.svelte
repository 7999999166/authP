<script>
  // Sales Entry Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4 d-flex align-items-center">
    <h1 class="h3 fw-bold me-auto" style="color: #03045e;">Sales Entry Form</h1>
    <div style:min-height="70px">
  <div class="collapse collapse-horizontal" id="collapseWidthExample">
    <div class="card card-body d-flex flex-row justify-content-center" style:min-width="70vw">
      <div class="form-check form-switch mx-2">
  <input class="form-check-input mx-3" type="checkbox" role="switch" id="switchCheckDefault">
  <label class="form-check-label" for="switchCheckDefault">Tax Feilds</label>
</div>
<div class="form-check form-switch mx-2">
  <input class="form-check-input mx-3" type="checkbox" role="switch" id="switchCheckChecked" checked>
  <label class="form-check-label" for="switchCheckChecked">Discount Feilds</label>
</div>
<div class="form-check form-switch mx-2">
  <input class="form-check-input mx-3" type="checkbox" role="switch" id="switchCheckDefault">
  <label class="form-check-label" for="switchCheckDefault">Other Charges Feilds</label>
</div>
<div class="form-check form-switch mx-2">
  <input class="form-check-input mx-3" type="checkbox" role="switch" id="switchCheckDefault">
  <label class="form-check-label" for="switchCheckDefault">Dispatch Details Feilds</label>
</div>
    </div>
  </div>
</div>
  <!-- svelte-ignore a11y_consider_explicit_label -->
  <!-- svelte-ignore a11y_missing_attribute -->
  <a role="button" class="px-4" data-bs-toggle="collapse" data-bs-target="#collapseWidthExample"   aria-expanded="false" aria-controls="collapseWidthExample">
   <i class="bi bi-sliders fs-4 fw-bold" style="color: #03045e;"></i>
  </a>
  

  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <!-- Left Column -->
        <div class="col-lg-4 col-md-6">
          <div class="d-flex flex-column gap-3">
            <div class="row align-items-center">
              <label
                for="delivery_challan"
                class="col-4 col-form-label text-secondary fw-medium"
                >Delivery Challan</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control bg-white text-center fw-semibold"
                  id="delivery_challan"
                  value="Auto Generated"
                  readonly
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="voucher_date"
                class="col-4 col-form-label text-secondary fw-medium"
                >Voucher Date</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control"
                  id="voucher_date"
                  value="16 November 2025"
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="due_date"
                class="col-4 col-form-label text-secondary fw-medium"
                >Due Date</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control"
                  id="due_date"
                  value="16 November 2025"
                />
              </div>
            </div>
          </div>
        </div>

        <!-- Middle Column -->
        <div class="col-lg-4 col-md-6">
          <div class="d-flex flex-column gap-3">
            <div class="row align-items-center">
              <label
                for="customer"
                class="col-4 col-form-label text-secondary fw-medium"
                >Customer/Cash</label
              >
              <div class="col-8">
                <input type="text" class="form-control" id="customer" />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="sales_account"
                class="col-4 col-form-label text-secondary fw-medium"
                >Sales Account</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control"
                  id="sales_account"
                  value="Sales"
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="po_no"
                class="col-4 col-form-label text-secondary fw-medium"
                >PO No.</label
              >
              <div class="col-8">
                <input type="text" class="form-control" id="po_no" />
              </div>
            </div>
          </div>
        </div>

        <!-- Right Column -->
        <div class="col-lg-4 col-md-6">
          <div class="d-flex flex-column gap-3">
            <div class="d-flex align-items-center gap-3">
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
            </div>
            <input
              type="text"
              class="form-control form-control-sm bg-white"
              value="DEFAULT"
              readonly
            />

            <div class="row align-items-center mt-2">
              <label
                for="place_of_supply"
                class="col-4 col-form-label text-secondary fw-medium"
                >Place Of Supply</label
              >
              <div class="col-8">
                <select class="form-select" id="place_of_supply">
                  <option>Delhi</option>
                  <option>Mumbai</option>
                  <option>Kolkata</option>
                </select>
              </div>
            </div>

            <div class="text-center mt-2">
              <small class="fw-semibold text-secondary"
                >Press ENTER to move forward</small
              >
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Item Entry & Table Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div
        class="d-flex flex-wrap align-items-center justify-content-between gap-3 mb-3"
      >
        <div
          class="d-flex align-items-center flex-grow-1"
          style="max-width: 400px;"
        >
          <label
            for="item_entry"
            class="fw-medium text-secondary me-2 text-nowrap">F9: Item</label
          >
          <input
            type="text"
            class="form-control"
            id="item_entry"
            placeholder="Press ENTER key to add item."
          />
        </div>
        <div class="small text-danger fw-medium text-end">
          DELETE: To Delete Row, Shift+UP/Down: To Rearrange Items
        </div>
      </div>

      <div class="small text-secondary mb-3 d-flex gap-3">
        <span>Units Left: 0</span>
        <a href="#" class="text-primary text-decoration-none"
          >Alt+F1: Warehouse</a
        >
        <a href="#" class="text-primary text-decoration-none"
          >Alt+F2: Item History</a
        >
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
                No items added.
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>

    <!-- Bottom Section -->
    <div class="row g-4">
      <!-- Left Column -->
      <div class="col-lg-4">
        <div class="d-flex flex-column gap-3">
          <div>
            <label for="narration" class="fw-medium text-secondary mb-1"
              >Narration</label
            >
            <small class="text-secondary d-block mb-1"
              >Ctrl+Enter for next line</small
            >
            <textarea class="form-control" id="narration" rows="4"></textarea>
          </div>

          <div class="d-flex flex-column gap-2">
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="discount" />
              <label class="form-check-label text-secondary" for="discount"
                >Discount</label
              >
            </div>
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="tax" />
              <label class="form-check-label text-secondary" for="tax"
                >Tax</label
              >
            </div>
            <div class="form-check">
              <input
                class="form-check-input"
                type="checkbox"
                id="other_charges"
              />
              <label class="form-check-label text-secondary" for="other_charges"
                >Other Charges</label
              >
            </div>
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="dispatch" />
              <label class="form-check-label text-secondary" for="dispatch"
                >Dispatch</label
              >
            </div>
          </div>
        </div>
      </div>

      <!-- Middle Column -->
      <div class="col-lg-4 d-flex flex-column justify-content-between">
        <div class="d-flex flex-column gap-3 align-items-end">
          <div class="d-flex align-items-center gap-2">
            <label for="amount" class="fw-medium text-secondary">Amount</label>
            <input
              type="text"
              class="form-control bg-light text-end"
              id="amount"
              value="0"
              readonly
              style="width: 150px;"
            />
          </div>
          <div class="d-flex align-items-center gap-2">
            <input
              type="text"
              class="form-control text-end"
              placeholder="Discount"
              style="width: 150px;"
            />
          </div>
          <div class="d-flex align-items-center gap-2">
            <input
              type="text"
              class="form-control text-end"
              placeholder="Tax"
              style="width: 150px;"
            />
          </div>
        </div>

        <div class="border border-secondary-subtle p-3 rounded mt-3">
          <p class="small fw-medium text-secondary mb-2">Discount & Tax</p>
          <div class="d-flex gap-3">
            <div class="form-check">
              <input
                class="form-check-input"
                type="radio"
                name="discount_tax"
                id="on_total"
                checked
              />
              <label
                class="form-check-label text-secondary small"
                for="on_total">On Total</label
              >
            </div>
            <div class="form-check">
              <input
                class="form-check-input"
                type="radio"
                name="discount_tax"
                id="per_item"
              />
              <label
                class="form-check-label text-secondary small"
                for="per_item">Per Item</label
              >
            </div>
          </div>
        </div>
      </div>

      <!-- Right Column -->
      <div class="col-lg-4 d-flex flex-column justify-content-end gap-3">
        <div class="d-flex align-items-center justify-content-end gap-2">
          <label for="round_off" class="fw-medium text-secondary"
            >Round Off</label
          >
          <input
            type="text"
            class="form-control text-end"
            id="round_off"
            value="0.00"
            style="width: 150px;"
          />
        </div>
        <div class="d-flex align-items-center justify-content-end gap-2">
          <label for="total_amount" class="fw-bold text-dark fs-5">Total</label>
          <input
            type="text"
            class="form-control bg-light text-end fw-bold fs-5"
            id="total_amount"
            value="0.00"
            readonly
            style="width: 150px;"
          />
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
      <button
        class="btn btn-primary d-flex align-items-center gap-1 fw-medium shadow-sm"
      >
        F12: Save
        <i class="bi bi-chevron-right small"></i>
      </button>
      <button class="btn btn-light border text-secondary fw-medium">
        Alt+F12: Save & View
      </button>
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
