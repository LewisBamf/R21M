
<style>
  
    .footer-content {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .footer-logo {
      display: flex;
      flex-direction: row;
      align-items: center;
      margin-bottom: 0.5rem;
      gap: 1rem;
    }

    .logo {
      width: 50px;
      height: auto;
  }

    .footer-description {
      font-size: 14px;
      margin: 10px 0;
    }


    .footer-bottom {
      border-top: 1px solid #444444;
      padding-top: 10px;
    }

    .footer-bottom-text {
      font-size: 12px;
    }

    .container {
      max-width: 900px;
      margin: 0 auto;
      padding: 2rem 1rem;
      padding-top: 0px;
  }

  .Links{
      display: flex;
      flex-direction: row;
      gap: 1rem;
  }

  
.social-media {
  margin-bottom: 3rem;
}

.social-media h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  color: var(--text);
  font-family: var(--heading-font);
}

.social-media ul {
  list-style: none;
  padding: 0;
  display: flex;
  flex-direction: row;
  gap: 1rem;
}

.social-media li {
  font-size: 1.25rem;
}

.social-media a {
  color: var(--primary);
  text-decoration: none;
}

.social-media a:hover {
  text-decoration: underline;
}

/* Style for the GitHub link */

.github-icon {
  width: 30px;
  height: 30px;
  fill: #333;
  transition: fill 0.3s ease;
}

.github-icon:hover {
  fill: #00FF75; /* Change icon color on hover */
}

.twitter-icon {
  width: 30px;
  height: 30px;
  fill: #333;
  transition: fill 0.3s ease;
}

.twitter-icon:hover {
  fill: #1DA1F2; /* Change icon color on hover */
}

.linkedin-icon {
  width: 30px;
  height: 30px;
  fill: #333;
  transition: fill 0.3s ease;
}

.linkedin-icon:hover {
  fill: #2867B2; /* Change icon color on hover */
}

.instagram-icon {
  width: 30px;
  height: 30px;
  fill: #333;
  transition: fill 0.3s ease;
}

.instagram-icon:hover {
  fill: #E4405F; /* Change icon color on hover */
}

@media (max-width: 600px) {
  .social-media h2 {
      font-size: 2rem;
  }

  .github-icon {
  fill: #00FF75; /* Change icon color on small devices */
}

.twitter-icon {
  fill: #1DA1F2; /* Change icon color on small devices */
}

.linkedin-icon {
  fill: #2867B2; /* Change icon color on small devices */
}

.instagram-icon {
  fill: #E4405F; /* Change icon color on small devices */
}
}
  </style>

  

  <div class="footer-content">
    <!-- Footer Logo and Description -->
    <div class="footer-logo">
      <img src={logo} alt="Logo" class="logo">
      <p class="footer-description">We are dedicated to providing the best services and products for our customers. Follow us on social media for the latest updates.</p>
    </div>
    
    <!-- Social Media Links -->
    <section class="social-media">
      <div class="container">
          <h2>Connect with Me</h2>
          <ul>
              <div class="Links">
              <li><a href="https://github.com/LewisBam" target="_blank" rel="noopener noreferrer" class="github-link"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="github-icon"><path d="M12 0C5.372 0 0 5.373 0 12c0 5.308 3.438 9.808 8.207 11.39.6.111.82-.26.82-.578 0-.286-.01-1.046-.015-2.057-3.338.725-4.04-1.606-4.04-1.606-.545-1.384-1.333-1.751-1.333-1.751-1.088-.743.083-.728.083-.728 1.205.084 1.838 1.236 1.838 1.236 1.07 1.836 2.809 1.305 3.493.998.107-.775.418-1.305.763-1.605-2.665-.303-5.466-1.332-5.466-5.928 0-1.31.469-2.381 1.24-3.222-.125-.303-.538-1.52.115-3.175 0 0 1.01-.323 3.3 1.228.957-.266 1.981-.399 3.001-.404 1.02.005 2.046.138 3.002.404 2.291-1.551 3.297-1.228 3.297-1.228.653 1.655.241 2.872.116 3.175.77.841 1.237 1.912 1.237 3.222 0 4.605-2.804 5.622-5.473 5.922.43.371.815 1.104.815 2.224 0 1.606-.015 2.913-.015 3.303 0 .319.22.694.825.578A12.026 12.026 0 0024 12c0-6.627-5.373-12-12-12z"/></svg></a></li>
              <li><a href="https://x.com/bamfordlewis9" target="_blank" rel="noopener noreferrer" class="twitter-link"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="twitter-icon"><path d="M18.901 1.153h3.68l-8.04 9.19L24 22.846h-7.406l-5.8-7.584-6.638 7.584H.474l8.6-9.83L0 1.154h7.594l5.243 6.932ZM17.61 20.644h2.039L6.486 3.24H4.298Z"/></svg></a></li>
              <li><a href="www.linkedin.com/in/lewis-bamford-802480287" target="_blank" rel="noopener noreferrer" class="linkedin-link"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="linkedin-icon"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg></a></li>
              <li><a href="https://www.instagram.com/lewis_bamford_cf/" target="_blank" rel="noopener noreferrer" class="instagram-link"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="instagram-icon"><path d="M7.0301.084c-1.2768.0602-2.1487.264-2.911.5634-.7888.3075-1.4575.72-2.1228 1.3877-.6652.6677-1.075 1.3368-1.3802 2.127-.2954.7638-.4956 1.6365-.552 2.914-.0564 1.2775-.0689 1.6882-.0626 4.947.0062 3.2586.0206 3.6671.0825 4.9473.061 1.2765.264 2.1482.5635 2.9107.308.7889.72 1.4573 1.388 2.1228.6679.6655 1.3365 1.0743 2.1285 1.38.7632.295 1.6361.4961 2.9134.552 1.2773.056 1.6884.069 4.9462.0627 3.2578-.0062 3.668-.0207 4.9478-.0814 1.28-.0607 2.147-.2652 2.9098-.5633.7889-.3086 1.4578-.72 2.1228-1.3881.665-.6682 1.0745-1.3378 1.3795-2.1284.2957-.7632.4966-1.636.552-2.9124.056-1.2809.0692-1.6898.063-4.948-.0063-3.2583-.021-3.6668-.0817-4.9465-.0607-1.2797-.264-2.1487-.5633-2.9117-.3084-.7889-.72-1.4568-1.3876-2.1228C21.2982 1.33 20.628.9208 19.8378.6165 19.074.321 18.2017.1197 16.9244.0645 15.6471.0093 15.236-.005 11.977.0014 8.718.0076 8.31.0215 7.0301.0839m.1402 21.6932c-1.17-.0509-1.8053-.2453-2.2287-.408-.5606-.216-.96-.4771-1.3819-.895-.422-.4178-.6811-.8186-.9-1.378-.1644-.4234-.3624-1.058-.4171-2.228-.0595-1.2645-.072-1.6442-.079-4.848-.007-3.2037.0053-3.583.0607-4.848.05-1.169.2456-1.805.408-2.2282.216-.5613.4762-.96.895-1.3816.4188-.4217.8184-.6814 1.3783-.9003.423-.1651 1.0575-.3614 2.227-.4171 1.2655-.06 1.6447-.072 4.848-.079 3.2033-.007 3.5835.005 4.8495.0608 1.169.0508 1.8053.2445 2.228.408.5608.216.96.4754 1.3816.895.4217.4194.6816.8176.9005 1.3787.1653.4217.3617 1.056.4169 2.2263.0602 1.2655.0739 1.645.0796 4.848.0058 3.203-.0055 3.5834-.061 4.848-.051 1.17-.245 1.8055-.408 2.2294-.216.5604-.4763.96-.8954 1.3814-.419.4215-.8181.6811-1.3783.9-.4224.1649-1.0577.3617-2.2262.4174-1.2656.0595-1.6448.072-4.8493.079-3.2045.007-3.5825-.006-4.848-.0608M16.953 5.5864A1.44 1.44 0 1 0 18.39 4.144a1.44 1.44 0 0 0-1.437 1.4424M5.8385 12.012c.0067 3.4032 2.7706 6.1557 6.173 6.1493 3.4026-.0065 6.157-2.7701 6.1506-6.1733-.0065-3.4032-2.771-6.1565-6.174-6.1498-3.403.0067-6.156 2.771-6.1496 6.1738M8 12.0077a4 4 0 1 1 4.008 3.9921A3.9996 3.9996 0 0 1 8 12.0077"/></svg></a></li>
              </div>
          </ul>
      </div>
  </section>
  
  <!-- Footer Bottom -->
  <div class="footer-bottom">
    <p class="footer-bottom-text">© 2024 Your Company. All rights reserved.</p>
  </div>
</div>

<script>
    import logo from '../../assets/logo.svg';
</script>