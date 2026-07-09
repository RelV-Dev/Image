Saat ini flow nya terganggu pada bagian resubmit file, yang dimana saat ini mendapatkan update ui dan beberapa button berubah, berikut adalah update nya:
Assignment detail sekarang berubah:
<div class="show-assignment-page with-updated-ui"><tii-workflow-lfw-student-show-assignment class="hydrated"></tii-workflow-lfw-student-show-assignment></div>
<tii-workflow-lfw-student-show-assignment class="hydrated"></tii-workflow-lfw-student-show-assignment>

Submit Button sekarang hanya button bukan seperti dulu:
<tii-workflow-student-summary-panel-new class="hydrated"><div slot="submission-action" class="submission-action"><tii-grn-button class="hydrated"><tii-grn-icon slot="icon-at-start" class="hydrated"></tii-grn-icon>Submit</tii-grn-button></div></tii-workflow-student-summary-panel-new>

Setelah button submit diklik:
<div class="upload-step" aria-live="polite"><main class="upload-container" part="upload-form-container"><tii-ing-dropzone class="hydrated"><!----><div part="overlay" class="tii-ing-dropzone__overlay" style="display: none;"></div><div class="upload-form-content" part="upload-form-container-content"><tdl-icon with-role="none" icon-name="cloud-upload" class="hydrated"></tdl-icon><span class="title initial">Drag and drop your file here</span><tii-ing-upload-button class="hydrated"><tdl-popover close-label="Close" class="hydrated"><tdl-button part="upload-form-container-button" class="hydrated"><tdl-icon slot="icon-at-end" icon-name="arrow-drop-down" with-role="none" class="hydrated"></tdl-icon>Browse Files</tdl-button><div slot="body"><h3 class="actions-heading">Upload a file from</h3><ul class="actions-menu"><li class="action-menu-item"><tdl-button part="upload-form-container-menu-browse-button" class="hydrated"><tdl-icon class="local-drive-icon hydrated" icon-name="folder" with-role="none"></tdl-icon><div class="button-label">Your device</div></tdl-button></li><li class="action-menu-item"><tdl-button part="upload-form-container-menu-google-drive-button" class="hydrated"><img class="google-drive-icon" src="https://cdn.turnitin.com/tii-lfw-components/prod/dist/long-form-writing/assets/logo_google_drive.png" alt="Google Drive™"><div class="button-label">Google Drive™</div></tdl-button></li><li class="action-menu-item"><tdl-button part="upload-form-container-menu-microsoft-onedrive-button" class="hydrated"><img class="microsoft-onedrive-icon" src="https://cdn.turnitin.com/tii-lfw-components/prod/dist/long-form-writing/assets/logo_microsoft_onedrive.png" alt="Microsoft OneDrive™"><div class="button-label">Microsoft OneDrive™</div></tdl-button></li></ul></div></tdl-popover></tii-ing-upload-button></div></tii-ing-dropzone></main><main class="upload-container" part="file-selected-container"><div class="file-submit"><tdl-text-input class="hydrated"><span slot="label">Submission title (required)</span></tdl-text-input></div></main><slot name="input"></slot><slot name="before-main-content"></slot><tii-ing-collapsible class="requirements hydrated"><span slot="heading"><slot name="requirements-heading">Upload Requirements</slot></span><slot name="requirements"></slot></tii-ing-collapsible><slot name="after-main-content"></slot></div>

Setelah itu seperti kemarin upload dan preview:
<slot name="form-submit-button-label">Upload and Preview</slot>

Loading dan menunggu preview seperti sebelumnya (sama seperti sebelumnya):
<div class="image-preview"><tdl-loading class="hydrated"></tdl-loading><span class="image-preview-headline">We are creating a preview of the file</span><span class="image-preview-description">Please wait for us to process a preview to ensure the correct file has been uploaded.</span></div>

Biasanya muncul file metadata setelah process preview selesai (Sama seperti sebelumnya):
<div class="file-metadata"><div class="file-metadata-item"><span class="file-metadata-item-label">Submission title</span><span class="file-metadata-item-value">Skripsi Bunga Soleha</span></div><div class="file-metadata-item"><span class="file-metadata-item-label">File size</span><span class="file-metadata-item-value">212.4 KB</span></div><div class="file-metadata-item"><span class="file-metadata-item-label">Word count</span><span class="file-metadata-item-value">5.769</span></div></div>

Ketika tidak muncul" cari button submit without preview atau biasanya button submit (Bagian ini masih sama seperti sebelumnya tidak usah diubah terlalu karena ui pada bagian ini gaberubah):
<div slot="custom-action-elements" class="form-actions"><tdl-button class="cancel-button hydrated">Cancel</tdl-button><tdl-button class="accept-button hydrated">Submit</tdl-button></div>

Button Resubmit (Letaknya sama seperti button Submit):
<tii-grn-button class="hydrated"><tii-grn-icon slot="icon-at-start" class="hydrated"></tii-grn-icon>Resubmit</tii-grn-button>

Tabel Data submission details ketika sudah ada file yang di submit:
<div class="multi-provider-data-display-container"><tii-mpdd-table class="hydrated"><table class="multi-provider-data-display-table"><caption class="tii-workflow-sr-only" aria-live="polite">Submission details: Displaying 1 row</caption><thead><tr><th scope="col" aria-sort="none" class="non-sortable" part="submission-th"><span class="column-name" part="submission-th-content">Title</span></th><th scope="col" aria-sort="none" class="non-sortable" part="submission-status-th"><span class="column-name" part="submission-status-th-content">Status</span></th><th scope="col" aria-sort="none" class="non-sortable" part="grade-display-th"><span class="column-name" part="grade-display-th-content">Grade</span></th><th scope="col" aria-sort="none" class="non-sortable" part="similarity-th"><span class="column-name" part="similarity-th-content">Similarity</span></th><th scope="col" aria-sort="none" class="centered non-sortable"><span class="column-name">Feedback</span></th><th scope="col" aria-sort="none" class="non-sortable"><span class="column-name">More</span></th></tr></thead><tbody><tr><td><tii-mpdd-title-display class="hydrated"></tii-mpdd-title-display></td><td><tii-mpdd-date-and-time-status-display class="hydrated"></tii-mpdd-date-and-time-status-display></td><td><tii-mpdd-grade-with-max-points-display class="hydrated"></tii-mpdd-grade-with-max-points-display></td><td><tii-mpdd-similarity-display class="hydrated"></tii-mpdd-similarity-display></td><td><tii-mpdd-comments-display class="hydrated"></tii-mpdd-comments-display></td><td><tii-workflow-student-actions-menu class="hydrated"></tii-workflow-student-actions-menu></td></tr></tbody></table></tii-mpdd-table></div>

Last Submission Confirmation:
<dialog id="tii-resubmission-last-submission-modal" tabindex="-1" aria-modal="" aria-labelledby="modal-title" class="tii-grn-modal backdrop-shade" open=""><section><header><h2 id="modal-title"><slot name="header"></slot></h2><div class="actions"><tii-grn-button id="close-button" icon-mode="icon-only" class="hydrated"><tii-grn-icon class="hydrated"></tii-grn-icon></tii-grn-button></div></header><div class="modal-content"><slot></slot></div><footer><div class="main-buttons"><slot name="cancel-button"></slot><slot name="accept-button"></slot></div></footer></section></dialog>

Yang berubah hanya pada bagian submission, untuk similarity viewer dan lain-lain masih tetap sama. Aku ingin kamu update flow nya agar mengikuti update UI Ini pada bagian submission, karena sekarang pada saat submission/resubmit akan muncul error:
08.34.10
resubmit: Resubmitting file
08.35.36
error: Upload file was selected, but no Upload/Confirm/Submit button was found
08.35.38
failed retry: Attempt failed, will retry: File was selected, but Turnitin did not show a usable upload confirmation button.

Karena upload nya tidak ditemukan oleh flow saat ini. Kamu pahami saja pada bagian ui modern flow saat ini, kemudian hanya ubah pada bagian submission, kode saat ini sudah sangat bagus, update saja agar dia mendeteksi UI yang baru. 