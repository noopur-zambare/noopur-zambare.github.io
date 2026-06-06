<!-- IMAGE WITH EXPAND BUTTON -->
<div style="margin-top: 10px; position: relative; width: 90%; margin-left: auto; margin-right: auto;">

  <img id="projectImage"
       src="/images/debiased_pruning/diagram.png"
       alt="Proposed Solution Diagram"
       style="
         width: 100%;
         display: block;
         border: 1px solid #ddd;
         border-radius: 4px;
         padding: 2px;
         background: #fff;
       ">

  <!-- EXPAND ICON -->
  <div onclick="openImageModal()"
       style="
         position: absolute;
         top: 8px;
         right: 8px;
         background: rgba(0,0,0,0.6);
         color: white;
         padding: 6px 8px;
         border-radius: 4px;
         cursor: pointer;
         font-size: 14px;
       ">
    ⤢
  </div>

</div>

<!-- FULLSCREEN MODAL -->
<div id="imageModal"
     onclick="closeImageModal()"
     style="
       display: none;
       position: fixed;
       z-index: 9999;
       left: 0;
       top: 0;
       width: 100%;
       height: 100%;
       background-color: rgba(0,0,0,0.85);
       justify-content: center;
       align-items: center;
     ">

  <img src="/images/debiased_pruning/diagram.png"
       style="
         max-width: 90%;
         max-height: 90%;
         border-radius: 6px;
         box-shadow: 0 0 20px rgba(0,0,0,0.5);
       ">

</div>

<script>
function openImageModal() {
  document.getElementById("imageModal").style.display = "flex";
}

function closeImageModal() {
  document.getElementById("imageModal").style.display = "none";
}
</script>