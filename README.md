# Sayabidevs-Internship

<style>
      body {
        font-family: Arial, sans-serif;
        background-color: #e9e0e0;
    }
      section {
          padding: 40px;
    }
      h1 {
          font-size: 24px;
          margin-bottom: 20px;
    }
      p {
          font-size: 16px;
          line-height: 1.5;
    }
      /* Add a CSS class for the fade-in animation */
      .animated {
          opacity: 0;
          transform: translateY(20px);
          transition: all 0.5s ease;
      }
      /* Use the class to trigger the animation on scroll */
      .animated.in-view {
          opacity: 1;
          transform: translateY(0);
      }
      /* Profile section styles */
      #profile {
          display: flex;
          align-items: center;
          background-color: #f5f5f5;
          padding: 20px;
      }
      .profile-image {
          border: 5px solid #333;
          border-radius: 50%;
          overflow: hidden;
          max-width: 150px;
          transition: transform 0.3s ease-in-out;
      }
      .profile-image img {
          display: block;
          width: 100%;
          height: auto;
      }
      .profile-info {
          margin-left: 20px;
      }
      .profile-info h2 {
          font-size: 24px;
      }
      /* Add a hover effect to the profile image */
      .profile-image:hover {
          transform: scale(1.1);
      }
      .contact-links a:hover {
          color: #0011fa;
      }
      .contact-links a {
          display: inline-block;
          padding: 5px 10px;
          background-color: #ff3c00;
          color: #fff; 
          text-decoration: none;
          border-radius: 5px;
          font-weight: bold;
          margin-right: 20px;
          margin-top: 10px;
          transition: color 0.3s;
          transition: background-color 0.3s;
      }
      .contact-links ul li {
          display: inline;
      }
    </style>
</head>
<body>
   <section id="profile">
        <div class="profile-image">
            <img src="Untitled design (6)-min.png" alt="Your Name">
        </div>
        <div class="profile-info">
            <h1>Hafiz Hassan Mustafa</h1>
            <p><b>AI/ML/DL Engineer</b></p>
            <p>Reliable candidate studied Mechanical Engineering and having hands-on experience in 
                Machine Learning & Deep Learning seeking an junior level position to expand skills and 
                gain valuable real-world experience.</p>
            <div class="contact-links">
                <ul>
                    <li><a href="https://mail.google.com/mail/u/0/#inbox:hassanqureshi700@gmail.com" target="_blank">Email</a></li>
                    <li><a href="https://github.com/Hassanmustafa786?tab=repositories" target="_blank">GitHub</a></li>
                    <li><a href="https://www.linkedin.com/in/hafiz-hassan-mustafa-692b391b4/" target="_blank">LinkedIn</a></li>
                </ul>
            </div>
        </div>
    </section>
    <script>
          $(window).scroll(function() {
                $('.animated').each(function(){
                    const position = $(this).offset().top;
                    const topOfScreen = $(window).scrollTop();
                    const windowHeight = $(window).height();
                    if (position < topOfScreen + windowHeight - 100) {
                        $(this).addClass('in-view');
                    }
                });
            });
    </script>
</body>
</html>
