<script>
  // Transaction View: Purchase
  // Layout based on purchase/purchase.png
</script>

<div class="container-fluid bg-white p-4 min-vh-100 font-monospace">
  <!-- Header -->
  <div class="text-center mb-4">
    <h4 class="fw-bold mb-1">
      AKHIL STAINLESS STEEL INDUSTRIES PRIVATE LIMITED
    </h4>
    <p class="mb-0 small">
      KH No. 93/13, Mundka Industrial Area, New Delhi - 110041
    </p>
    <p class="mb-0 small">
      <i class="bi bi-envelope me-1"></i>assipl023@gmail.com,
      <i class="bi bi-telephone me-1"></i>9999995595
    </p>
    <p class="mb-0 small fw-bold">GSTIN: 07AAYCA5420B1ZS</p>
  </div>

  <h5 class="text-center fw-bold text-uppercase mb-3">PURCHASE</h5>

  <!-- Purchase Details -->
  <div class="border border-dark mb-0">
    <div class="row g-0">
      <!-- Left Column: Bill From -->
      <div class="col-8 border-end border-dark p-2">
        <div class="fw-bold text-decoration-underline mb-1">Bill From:</div>
        <div class="fw-bold">JINDAL POLYMERS</div>
        <div>I-214, SECTOR-3, DSIIDC INDL AREA, BAWANA, New Delhi</div>
        <div>Delhi</div>
        <div><span class="fw-bold">GSTIN:</span> 07ADMPJ2851R1ZW</div>
        <div><span class="fw-bold">Place Of Supply:</span> 07-Delhi</div>
      </div>
      <!-- Right Column: Info -->
      <div class="col-4 p-2">
        <div class="mb-1 text-end">
          <span class="fw-bold">Purchase No:</span> PUR-208
        </div>
        <div class="mb-1 text-end">
          <span class="fw-bold">Date:</span> 19-11-2025
        </div>
        <div class="mb-1 text-end">
          <span class="fw-bold">Supplier Invoice No:</span> 2025-26/556
        </div>
      </div>
    </div>

    <!-- Item Table -->
    <div class="border-top border-dark">
      <table
        class="table table-bordered border-dark mb-0 text-center"
        style="font-size: 0.9rem;"
      >
        <thead class="table-light">
          <tr>
            <th style="width: 40px;">#</th>
            <th class="text-start">Description</th>
            <th style="width: 70px;">HSN</th>
            <th style="width: 90px;">QTY</th>
            <th style="width: 60px;">Units</th>
            <th style="width: 90px;">Rate</th>
            <th style="width: 60px;">Per</th>
            <th style="width: 140px;">Amount</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1</td>
            <td class="text-start">PLASTIC PACKING MATERIAL</td>
            <td>7323</td>
            <td>1148.14</td>
            <td>kg</td>
            <td>127.00</td>
            <td>kg</td>
            <td class="text-end">1,45,813.78</td>
          </tr>
          <!-- Empty rows/spacing -->
          <tr style="height: 80px;">
            <td colspan="8"></td>
          </tr>
        </tbody>
        <tfoot class="border-top border-dark">
          <tr>
            <td colspan="7" class="text-end fw-bold">Subtotal</td>
            <td class="text-end fw-bold">1,45,813.78</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">CGST@9%</td>
            <td class="text-end fw-bold">13,123.24</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">SGST@9%</td>
            <td class="text-end fw-bold">13,123.24</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">Round Off</td>
            <td class="text-end fw-bold">-0.26</td>
          </tr>
          <tr>
            <td colspan="3" class="text-start fw-bold border-end-0">Total</td>
            <td class="fw-bold border-start-0 border-end-0">1,148.14</td>
            <td colspan="3" class="border-start-0"></td>
            <td class="text-end fw-bold">INR 1,72,060.00</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">Paid</td>
            <td class="text-end fw-bold">INR 0.00</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold border-bottom-0">Balance</td
            >
            <td class="text-end fw-bold text-danger border-bottom-0"
              >INR 1,72,060.00</td
            >
          </tr>
        </tfoot>
      </table>
    </div>
  </div>

  <!-- Footer Info -->
  <div class="mt-2">
    <p class="mb-1">
      <span class="fw-bold">Amount (in words) :</span> INR One Hundred Seventy Two
      Thousand Sixty Only
    </p>
    <p class="mb-4"><span class="fw-bold">Total Tax:</span> 26246.48</p>

    <div class="row mt-5">
      <div class="col-8">
        <div class="small">
          <p class="mb-1">
            We declare that this invoice shows the actual price of the goods
            described and that all particulars are true and correct.
          </p>
        </div>
      </div>
      <div
        class="col-4 text-end d-flex flex-column justify-content-end align-items-end"
      >
        <div
          class="border border-secondary rounded-circle d-flex align-items-center justify-content-center mb-2"
          style="width: 100px; height: 100px; opacity: 0.5;"
        >
          <!-- Placeholder for Stamp/Signature -->
          <span
            class="small text-muted text-center"
            style="transform: rotate(-15deg);"
            >AKHIL STAINLESS<br />STEEL IND P. LTD</span
          >
        </div>
        <p class="fw-bold mb-0">Authorized Signatory</p>
      </div>
    </div>

    <div class="text-center mt-5 small text-muted">
      This is computer generated invoice
    </div>
  </div>
</div>

<style>
  .font-monospace {
    font-family: "Courier New", Courier, monospace !important;
  }
  .table-bordered > :not(caption) > * > * {
    border-width: 1px;
  }
  .small {
    font-size: 0.85rem;
  }
</style>
