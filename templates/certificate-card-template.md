1️⃣ Open the template file

From your repo root:

code templates/certificate-card-template.md

(or open it in VS Code manually)

2️⃣ Paste this content into the file
# Certificate Card Template

Use this template when adding a new certificate to `index.html`.

Update the following fields:

- `id`
- certificate title
- PDF filename

---

## HTML Card Template

```html
<div class="card">
  <h3 id="certificate-id">
    <a
      href="CertificateFile.pdf"
      target="_blank"
      rel="noopener noreferrer"
    >
      Certificate Title (Provider)
    </a>
  </h3>

  <object
    class="viewer"
    data="CertificateFile.pdf#toolbar=0&view=FitH"
    type="application/pdf"
  >
    <embed
      class="viewer"
      src="CertificateFile.pdf#toolbar=0&view=FitH"
      type="application/pdf"
    />

    PDF viewer not available.
    <a
      href="CertificateFile.pdf"
      target="_blank"
      rel="noopener noreferrer"
    >
      Open full size
    </a>
  </object>

  <p class="links">
    <a
      href="CertificateFile.pdf"
      target="_blank"
      rel="noopener noreferrer"
    >
      Open full size
    </a>
  </p>
</div>
3️⃣ Steps to Add a New Certificate
1️⃣ Add the PDF file

Place the certificate PDF in the repo root.

Example:

NewCertificate_Codecademy.pdf
2️⃣ Copy the template block

Copy the HTML card above and paste it into:

index.html

inside the .grid section.

3️⃣ Update three things

Change:

certificate-id
Certificate Title (Provider)
CertificateFile.pdf

Example:

<h3 id="javascript-course">
  <a href="JavaScriptCourse_Codecademy.pdf">
4️⃣ Update README

Add the certificate to the list:

- 📄 [Certificate Title (Provider)](https://cg112358.github.io/certificates/CertificateFile.pdf)
5️⃣ Commit changes
git add index.html README.md CertificateFile.pdf
git commit -m "docs: add <certificate name>"
git push
4️⃣ Save and commit the template

After pasting the template:

git add templates/certificate-card-template.md
git commit -m "docs: add certificate card template"
git push
Resulting repo structure
certificates/
│
├── index.html
├── README.md
├── *.pdf
│
└── templates/
    └── certificate-card-template.md