## youqishan

<!-- 1. My virtual photo: Click to toggle show/hide -->
<img 
  src="./profile_photo.jpg" alt="My virtual photo" width="300" style="cursor: pointer; display: block; margin: 0 auto; border-radius: 8px;" onclick="toggleAboutMe()">

---

## Welcome
My name is Yuhao Liu. I am an IBI1 student at the Zhejiang University – University of Edinburgh (ZJE) Institute.

<!-- 2. About Me: Hidden by default, displayed only after clicking the photo -->
<div id="about-me-section" style="display: none; margin-top: 20px;">
  
## About Me
  I like reading online novels very much. Nice to meet you! 😊
</div>

<!-- 3. JavaScript：Control display and hide -->
<script>
function toggleAboutMe() {
  // get section "About Me"
  const aboutSection = document.getElementById("about-me-section");
  
  if (aboutSection.style.display === "none") {
    aboutSection.style.display = "block"; // from hide to display
  } else {
    aboutSection.style.display = "none"; // form display to hide
  }
}
</script>
