<style>
.tut-img {
  max-width: 250px;
  width: 100%;
  height: auto;
  border-radius: 8px;
  cursor: zoom-in;
  display: block;
  margin: 10px 0;
}
.lightbox-overlay {
  display: none;
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  background: rgba(0,0,0,0.85);
  z-index: 9999;
  justify-content: center;
  align-items: center;
  cursor: zoom-out;
}
.lightbox-overlay.active {
  display: flex;
}
.lightbox-overlay img {
  max-width: 95%;
  max-height: 95%;
  border-radius: 6px;
}
</style>

<p><strong>How to add Seerr as an iPhone Applet:</strong></p>
<p>On your iPhone's Safari app, navigate to the <a href="https://request.willystation.com">WillyStation Request Site</a></p>
<p>Then, do the following:</p>
<p><em>note that the app "Jellyseerr" has been renamed to "Seerr"</em></p>

<img class="tut-img" src="https://i.imgur.com/eqk8N0l.png" onclick="openLightbox(this.src)">
<img class="tut-img" src="https://i.imgur.com/deqzwNp.jpeg" onclick="openLightbox(this.src)">
<img class="tut-img" src="https://i.imgur.com/c8E8GTz.png" onclick="openLightbox(this.src)">

<div class="lightbox-overlay" id="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="">
</div>

<script>
function openLightbox(src) {
  document.getElementById('lightbox-img').src = src;
  document.getElementById('lightbox').classList.add('active');
}
function closeLightbox() {
  document.getElementById('lightbox').classList.remove('active');
}
</script>
