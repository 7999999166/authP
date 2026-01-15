<script>
  // Transaction View: Sale (Invoice)
  // Layout based on sale/invoice.png
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

  <h5 class="text-center fw-bold text-decoration-underline mb-3">
    Tax Invoice
  </h5>

  <!-- Invoice Details -->
  <div class="border border-dark mb-0">
    <div class="row g-0">
      <!-- Left Column -->
      <div class="col-6 border-end border-dark p-2">
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 130px;">Invoice No</span>
          <span>: GST/25-26/800</span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 130px;">Date</span>
          <span>: 16-12-2025</span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 130px;"
            >Purchase Order No</span
          >
          <span>: </span>
        </div>
      </div>
      <!-- Right Column -->
      <div class="col-6 p-2">
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 100px;">Transport</span>
          <span>: </span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 100px;">Vehicle No.</span>
          <span>: </span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 100px;">GR/RR No.</span>
          <span>: </span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 100px;">e-Way Bill No.</span>
          <span>: 741588427901</span>
        </div>
      </div>
    </div>

    <!-- Parties -->
    <div class="row g-0 border-top border-dark">
      <!-- Billed To -->
      <div class="col-6 border-end border-dark">
        <div
          class="fw-bold text-center border-bottom border-dark py-1 bg-light"
        >
          Details of Receiver (Billed To)
        </div>
        <div class="p-2">
          <div class="fw-bold">KRISHI RASAYAN EXPORTS PVT LTD</div>
          <div>
            Phase-1, SIDCO, Ist Parallel Road, Industrial Growth Centre, Samba
          </div>
          <div>Jammu & Kashmir</div>
          <div>India</div>
          <div>184121</div>
          <div class="mt-1">
            <span class="fw-bold">GSTIN:</span> 01AACC K4124G1Z7
          </div>
          <div>
            <span class="fw-bold">Place Of Supply:</span> 01-Jammu & Kashmir
          </div>
        </div>
      </div>
      <!-- Shipped To -->
      <div class="col-6">
        <div
          class="fw-bold text-center border-bottom border-dark py-1 bg-light"
        >
          Details of Consignee (Shipped To)
        </div>
        <div class="p-2">
          <div class="fw-bold">KRISHI RASAYAN EXPORTS PVT LTD</div>
          <div>
            Phase-1, SIDCO, Ist Parallel Road, Industrial Growth Centre, Samba
          </div>
          <div>Jammu & Kashmir</div>
          <div>India</div>
          <div>184121</div>
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
            <th style="width: 50px;">#</th>
            <th class="text-start">Description</th>
            <th style="width: 80px;">HSN</th>
            <th style="width: 100px;">QTY</th>
            <th style="width: 80px;">Units</th>
            <th style="width: 100px;">Rate</th>
            <th style="width: 80px;">Per</th>
            <th style="width: 150px;">Amount</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1</td>
            <td class="text-start">
              <div class="fw-bold">TS DABBA</div>
              <div class="small">450 PCS.</div>
            </td>
            <td>7323</td>
            <td>416.00</td>
            <td>kg</td>
            <td>236.00</td>
            <td>kg</td>
            <td class="text-end">98,176.00</td>
          </tr>
          <!-- Empty rows for spacing -->
          <tr style="height: 100px;">
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
          </tr>
        </tbody>
        <tfoot class="border-top border-dark">
          <tr>
            <td colspan="7" class="text-end fw-bold">Subtotal</td>
            <td class="text-end fw-bold">98,176.00</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">IGST@5%</td>
            <td class="text-end fw-bold">4,908.80</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">Round Off</td>
            <td class="text-end fw-bold">0.20</td>
          </tr>
          <tr>
            <td colspan="3" class="text-start fw-bold border-end-0">Total</td>
            <td class="fw-bold border-start-0 border-end-0">416.00</td>
            <td colspan="3" class="border-start-0"></td>
            <td class="text-end fw-bold">INR 1,03,085.00</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">Paid</td>
            <td class="text-end fw-bold">INR 0.00</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold border-bottom-0">Balance</td
            >
            <td class="text-end fw-bold text-danger border-bottom-0"
              >INR 1,03,085.00</td
            >
          </tr>
        </tfoot>
      </table>
    </div>
  </div>

  <!-- Footer Info -->
  <div class="mt-2">
    <p class="mb-1">
      <span class="fw-bold">Amount (in words) :</span> INR One Hundred Three Thousand
      Eighty Five Only
    </p>
    <p class="mb-4"><span class="fw-bold">Total Tax:</span> 4908.80</p>

    <div class="row mt-4">
      <div class="col-6">
        <p class="mb-1 fw-bold">Account Number : 235605001136</p>
        <p class="mb-1 fw-bold">Bank : ICICI Bank</p>
        <p class="mb-1 fw-bold">IFSC CODE : ICIC0002356</p>

        <div class="mt-4 small">
          <p class="mb-1">1. Goods once sold will not be taken back.</p>
          <p class="mb-1">
            2. Interest @18% P.a. will be charged if the payment is not made
            with in the stipulated time.
          </p>
          <p class="mb-1">3. Subject to "Delhi" Jurisdiction only.</p>
        </div>
      </div>
      <div
        class="col-6 text-end d-flex flex-column justify-content-end align-items-end"
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

    <div class="text-center mt-4 small text-muted">
      This is computer generated invoice
    </div>
  </div>
</div>

<style>
  /* Print-like styling adjustments */
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
