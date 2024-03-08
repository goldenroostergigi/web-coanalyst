<template>
  <div class="footer-container">
    <div class="made-in">Made in Mexico City. 2024.</div>
    <div class="social-links-container">
      <div class="social-links">
        <a href="https://www.lesswrong.com" class="link">LessWrong</a> |
        <a href="https://twitter.com" class="link">Twitter</a> |
        <a href="https://instagram.com" class="link">Instagram</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style scoped>
.footer-container {
  width: 100%;
  height: auto; /* Adjust height to auto for better flexibility */
  display: flex;
  flex-direction: row; /* Default direction */
  justify-content: space-between;
  align-items: center;
  padding: 2em 4em; /* Adjust padding as needed */
  box-sizing: border-box;
  flex-wrap: wrap; /* Allow items to wrap in smaller screens */
}

.social-links {
  display: flex;
  gap: 10px; /* Adjust gap as needed */
  flex-wrap: wrap; /* Allow links to wrap */
}

.link {
  text-decoration: none;
  color: inherit; /* Removes the default hyperlink color */
}

@media (max-width: 768px) {
  .footer-container {
    flex-direction: column;
    padding: 2em;
    font-size: 0.8em;
    align-items: center; /* Center items horizontally */
  }
  .made-in, .social-links-container, .social-links {
    width: 100%;
    justify-content: center; /* This will center the flex items horizontally */
    text-align: center; /* Center the text for each link */
  }
  .social-links {
    margin-top: 1em; /* Add some space between the text and the links */
    display: flex; /* Ensure this is a flex container */
    justify-content: center; /* Center flex items (links) */
  }
}

</style>
