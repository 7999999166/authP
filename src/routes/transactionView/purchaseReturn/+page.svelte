<script>
  // Transaction View: Purchase Return (Debit Note)
  // Layout based on purchaseReturn/debit note.png
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

  <h5 class="text-center fw-bold mb-3">Debit Note</h5>

  <!-- Details Box -->
  <div class="border border-dark mb-0">
    <div class="row g-0">
      <!-- Left Column: To -->
      <div class="col-8 border-end border-dark p-2">
        <div class="fw-bold text-decoration-underline mb-1">To:</div>
        <div class="fw-bold">D.D. METALS</div>
        <div>
          HOUSE NO.17, BLOCK-A, WAZIRPUR INDUSTRIAL AREA, North West Delhi
        </div>
        <div>Delhi</div>
        <div><span class="fw-bold">GSTIN:</span> 07ABSPK0042R1Z6</div>
        <div><span class="fw-bold">Place Of Supply:</span> 07-Delhi</div>
      </div>
      <!-- Right Column: Info -->
      <div class="col-4 p-2">
        <div class="mb-1 text-end">
          <span class="fw-bold">Debit Note No:</span> PRR1
        </div>
        <div class="mb-1 text-end">
          <span class="fw-bold">Date:</span> 21-02-2025
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
            <th style="width: 100px;">HSN</th>
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
            <td class="text-start">
              <div class="fw-bold">SS COIL</div>
              <div class="fst-italic mt-1 border-top border-secondary pt-1">
                <span class="fw-medium">Remarks:</span>
              </div>
              <div class="fst-italic">LOW QUALITY MATERIAL</div>
              <div class="fst-italic">
                DEBIT NOTE ISSUED AGAINST BILL NO-DDM/2024-25/641
              </div>
            </td>
            <td>72193490</td>
            <td>4165.00</td>
            <td>kg</td>
            <td>138.00</td>
            <td>kg</td>
            <td class="text-end">5,74,770.00</td>
          </tr>
          <!-- Empty rows/spacing -->
          <tr style="height: 100px;">
            <td colspan="8"></td>
          </tr>
        </tbody>
        <tfoot class="border-top border-dark">
          <tr>
            <td colspan="7" class="text-end fw-bold">Subtotal</td>
            <td class="text-end fw-bold">5,74,770.00</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">CGST@9%</td>
            <td class="text-end fw-bold">51,729.30</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">SGST@9%</td>
            <td class="text-end fw-bold">51,729.30</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">Round Off</td>
            <td class="text-end fw-bold">0.40</td>
          </tr>
          <tr>
            <td colspan="3" class="text-start fw-bold border-end-0">Total</td>
            <td class="fw-bold border-start-0 border-end-0">4,165.00</td>
            <td colspan="3" class="border-start-0"></td>
            <td class="text-end fw-bold">INR 6,78,229.00</td>
          </tr>
        </tfoot>
      </table>
    </div>
  </div>

  <!-- Footer Info -->
  <div class="mt-2">
    <p class="mb-1">
      <span class="fw-bold">Amount (in words) :</span> INR Six Hundred Seventy Eight
      Thousand Two Hundred Twenty Nine Only
    </p>

    <div class="row mt-5">
      <div class="col-8">
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
