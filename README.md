<button id="open-modal-button">Open Modal</button>

<div id="modal-container" class="modal-container">
  <div class="modal-content">
    <h2>Modal Title</h2>
    <p>Modal Content</p>
    <button id="close-modal-button">Close</button>
  </div>
</div>

.modal-container {
  display: none; /* Initially hidden */
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5); /* Black overlay */
  z-index: 999; /* Place the modal on top of other content */
}

.modal-content {
  background-color: white;
  margin: 10% auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  width: 500px;
}



const openModalButton = document.getElementById('open-modal-button');
const modalContainer = document.getElementById('modal-container');
const closeModalButton = document.getElementById('close-modal-button');

openModalButton.addEventListener('click', () => {
  modalContainer.style.display = 'block';
});

closeModalButton.addEventListener('click', () => {
  modalContainer.style.display = 'none';
});
