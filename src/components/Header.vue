<script setup>
</script>

<template>
<header class="main-header">
  <img
    class="logo"
    src="https://t4.ftcdn.net/jpg/06/90/82/69/360_F_690826931_H2Gxvlm26y12tkrcZ3xAfFPphmdNRVjn.jpg"
    alt="Kinema Logo"
  />
  <input class="searchbar" placeholder="Search" />
</header>
  </template>

<style scoped>
/* Header Styling */
.main-header {
  display: flex;
  align-items: center;
  justify-content: center; /* Center all content horizontally */
  padding: 10px 20px;
  background-color: #131313; /* Dark background */
  color: white;
  font-family: Arial, sans-serif;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Subtle shadow */
  position: relative; /* Allow absolute positioning for the logo */
}

/* Logo Styling */
.logo {
  height: 50px; /* Adjust logo height */
  border-radius: 50%; /* Optional rounded logo */
  position: absolute; /* Position logo absolutely */
  left: 20px; /* Align logo to the left */
}

/* Search Bar Styling */
.searchbar {
  width: 100%; /* Full width */
  max-width: 600px; /* Limit the maximum width */
  padding: 8px 12px; /* Add padding inside the search bar */
  font-size: 1rem; /* Font size for input text */
  border: 1px solid #ccc; /* Light border */
  border-radius: 5px; /* Rounded corners */
  outline: none; /* Remove focus outline */
  transition: border-color 0.3s, box-shadow 0.3s; /* Smooth focus transition */
}

.searchbar:focus {
  border-color: #3498db; /* Blue border on focus */
  box-shadow: 0 0 5px rgba(52, 152, 219, 0.5); /* Subtle glow on focus */
}

@media (max-width: 600px) {
  .main-header {
    flex-direction: column; /* Stack logo and search bar vertically */
    align-items: center;
  }

  .searchbar {
    width: 90%; /* Adjust width for smaller screens */
    margin-top: 10px; /* Add spacing between logo and search bar */
  }
}
</style>