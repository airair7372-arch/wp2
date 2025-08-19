document.addEventListener("DOMContentLoaded", function () {
  // Combined tab functionality
  const tabs = document.querySelectorAll(".tab-btn");
  const cards = document.querySelectorAll(".event-card");
  const eventContainers = document.querySelectorAll("[id^='event-cards-']");
  const tabButtons = document.querySelectorAll("[id^='tab-btn-']");

  function school_classroom_handleTabDisplay(index) {
    // Handle main tab switching
    eventContainers.forEach((container, i) => {
      const isActive = i === index;
      container.style.display = isActive ? 'block' : 'none';
      container.classList.toggle('active', isActive);
    });

    // Update tab button states
    tabButtons.forEach((btn, i) => btn.classList.toggle('active', i === index));
  }

  // Event listeners for category filtering
  tabs.forEach(tab => {
    tab.addEventListener("click", function() {
      tabs.forEach(t => t.classList.remove("active"));
      this.classList.add("active");

      const category = this.getAttribute("data-category");
      cards.forEach(card => {
        card.style.display = (category === "all" || category === card.getAttribute("data-category")) 
          ? "block" 
          : "none";
      });
    });
  });

  // Event listeners for tab switching
  tabButtons.forEach((btn, index) => {
    btn.addEventListener('click', () => school_classroom_handleTabDisplay(index));
  });

  // Initialize first tab
  school_classroom_handleTabDisplay(0);
   wow = new WOW(
    {
    boxClass:     'wow',      // default
    animateClass: 'animated', // default
    offset:       0,          // default
    mobile:       true,       // default
    live:         true        // default
  }
  )
  wow.init();
});

// Slider Js

jQuery(document).ready(function(){
  var owl = jQuery('.owl-carousel');
    owl.owlCarousel({
    margin: 20,
    nav: false,
    autoplay: true,
    lazyLoad: true,
    autoplayTimeout: 3000,
    loop: true,
    dots: true,
    navText: ['<i class="fas fa-chevron-left"></i>','<i class="fas fa-chevron-right"></i>'],
    responsive: {
      0: {
        items: 1,
        nav: false
      },
      600: {
        items: 1
      },
      1000: {
        items: 1
      }
    },
    autoplayHoverPause: true,
    mouseDrag: true
  });
});