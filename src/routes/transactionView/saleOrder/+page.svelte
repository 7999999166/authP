<script>
  // Transaction View: Sale Order (Proforma Invoice)
  // Layout based on saleOrder/sale order.png
</script>

<div class="container-fluid bg-white p-4 min-vh-100 font-monospace">
  <!-- Header -->
  <div class="text-center mb-4">
    <h4 class="fw-bold mb-1">
      AKHIL STAINLESS STEEL INDUSTRIES PRIVATE LIMITED
    </h4>
    <p class="mb-0 small">
      KH No. 93/13, Mundka Industrial Area, New Delhi -110041
    </p>
    <p class="mb-0 small">
      <i class="bi bi-envelope me-1"></i>assipl023@gmail.com,
      <i class="bi bi-telephone me-1"></i>9999995595
    </p>
    <p class="mb-0 small fw-bold">GSTIN: 07AAYCA5420B1ZS</p>
  </div>

  <h5 class="text-center fw-bold mb-3">Proforma Invoice</h5>

  <!-- Details Box -->
  <div class="border border-dark mb-0">
    <div class="row g-0">
      <!-- Left Column: To -->
      <div class="col-8 border-end border-dark p-2">
        <div class="fw-bold text-decoration-underline mb-1">To:</div>
        <div class="fw-bold">MAGNUM MACHINES & TOOLS</div>
        <div>
          191, First Floor, Khasra No. 31/23, Matiyala Extension, Behind DPS,
          Sector 3, Dwarka, New Delhi
        </div>
        <div>Delhi-110059</div>
        <div><span class="fw-bold">GSTIN:</span> 07ABOFM1262D1ZE</div>
      </div>
      <!-- Right Column: Info -->
      <div class="col-4 p-2">
        <div class="mb-1 text-end">
          <span class="fw-bold">Proforma Invoice No:</span> PI2
        </div>
        <div class="mb-1 text-end">
          <span class="fw-bold">Dated:</span> 19-04-2024
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
            <th style="width: 100px;">Rate</th>
            <th style="width: 140px;">Amount</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1</td>
            <td class="text-start">
              <div class="fw-bold">Deep Kadhai 07 (2mm)</div>
            </td>
            <td>7323</td>
            <td>234.00 pc</td>
            <td>345.00</td>
            <td class="text-end">80,730.00</td>
          </tr>
          <!-- Empty rows/spacing -->
          <tr style="height: 100px;">
            <td colspan="6"></td>
          </tr>
        </tbody>
        <tfoot class="border-top border-dark">
          <tr>
            <td colspan="5" class="text-end fw-bold">Sub Total</td>
            <td class="text-end fw-bold">80,730.00</td>
          </tr>
          <tr>
            <td colspan="5" class="text-end fw-bold">Discount</td>
            <td class="text-end fw-bold">-8,073.00</td>
          </tr>
          <tr>
            <td colspan="5" class="text-end fw-bold">CGST@1.5% (1.50 %)</td>
            <td class="text-end fw-bold">1,089.86</td>
          </tr>
          <tr>
            <td colspan="5" class="text-end fw-bold">SGST@1.5% (1.50 %)</td>
            <td class="text-end fw-bold">1,089.86</td>
          </tr>
          <tr>
            <td colspan="5" class="text-end fw-bold">Round Off</td>
            <td class="text-end fw-bold">0.28</td>
          </tr>
          <tr>
            <td colspan="3" class="text-start fw-bold border-end-0">Total</td>
            <td class="fw-bold border-start-0 border-end-0">234.00</td>
            <td class="border-start-0"></td>
            <td class="text-end fw-bold">INR 74,837.00</td>
          </tr>
        </tfoot>
      </table>
    </div>
  </div>

  <!-- Footer Info -->
  <div class="mt-2">
    <p class="mb-1">
      <span class="fw-bold">Amount (in words) :</span> INR Seventy Four Thousand
      Eight Hundred Thirty Seven Only
    </p>

    <div class="row mt-5">
      <div class="col-8">
        <div class="small">
          <p class="mb-0 fw-bold">E. & O.E.</p>
          <p class="mb-0">1. Goods once sold will not be taken back.</p>
          <p class="mb-0">
            2. Interest @18% P.a. will be charged if the payment is not made
            with in the stipulated time.
          </p>
          <p class="mb-0">3. Subject to "Delhi" Jurisdiction only.</p>
          <br /><br />
          <p class="min-w text-muted">
            This is not an invoice, only an estimate of the goods/services
            described above. Invoice will be generated after acceptance of this
            estimate.
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
