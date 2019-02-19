<template>
  <div id="app">
    <header>
      <!--TODO - General Sizing of elements seems off.-->
      <a id="header-logo" href="/"><img src="img/logo.png" alt="Platt Logo"></a>

      <div id="header-nav">
        <!--TODO - Add profile as vue component, it will need to know when to display badge.-->
        <!--TODO - Hamburger Nav Aside.-->

        <ul>
          <li>
            <a href="#search"><img class="icon icon-white-search" src="ic/white/ic_search.png" alt="Search"></a>
          </li>
          <li>
            <a href="#search"><img class="icon icon-white-shopping-cart" src="ic/white/ic_shopping_cart.png" alt="Shopping Cart"></a>
          </li>
          <li>
            <a href="#search"><img class="icon icon-white-person" src="ic/white/ic_person.png" alt="Profile"></a>
          </li>
          <li>
            <a href="#search"><img class="icon icon-white-menu" src="ic/white/ic_menu.png" alt="Menu"></a>
          </li>
        </ul>
      </div>

      <!--TODO - Implement Search.-->
      <div class="search-wrapper">
        <form class="search-form" action="#">
          <input type="text" placeholder="What Are You Looking For?">
          <button class="button-unstyled">
            <img src="ic/black/ic_search.png" alt="Search">
          </button>
        </form>
      </div>
    </header>

    <div id="categories-wrapper" class="categories-wrapper">
      <!--TODO - Make category containers vue components-->
      <!--TODO - Spacing and borders - Might need it to be a sub grid element to line up the right way-->

      <div class="categories-element categories-element-all">
        <img src="ic/black/ic_categories.png" alt="All Categories Icon">
        <strong><h2>Shop all categories</h2></strong>
        <img class="categories-element-arrow" src="ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="ic/black/ic_playlist_add_check.png" alt="My Catalog Icon">
        <h2>My Catalog</h2>
        <img class="categories-element-arrow" src="ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="ic/black/ic_list.png" alt="My List Icon">
        <h2>My List</h2>
        <img class="categories-element-arrow" src="ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="ic/green/ic_chat_active.png" alt="Chat Active Icon">
        <h2>Live Help</h2>
        <img class="categories-element-arrow" src="ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="ic/black/ic_check_circle.png" alt="PIM">
        <h2>PIM</h2>
        <img class="categories-element-arrow" src="ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="ic/black/ic_playlist_add_check.png" alt="Account Icon">
        <h2>Account</h2>
        <img class="categories-element-arrow" src="ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="ic/black/ic_place.png" alt="Branch Locations">
        <h2>Branch Locations</h2>
        <img class="categories-element-arrow" src="ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>
    </div>


    <!--SHOW ONLY ON MOBILE-->
    <div class="section-container functionality-circle-container show-phone">
      <!--TODO - Make these components-->
      <div class="functionality-circle-wrapper">
        <div class="functionality-circle drop-shadow">
          <img src="ic/green/ic_line_style.png" alt="Categories">
        </div>
        <span>Categories</span>
      </div>

      <div class="functionality-circle-wrapper">
        <div class="functionality-circle drop-shadow">
          <img src="ic/green/ic_search.png" alt="Search">
        </div>
        <span>Search</span>
      </div>

      <div class="functionality-circle-wrapper">
        <div class="functionality-circle drop-shadow">
          <img src="ic/green/ic_scanner.png" alt="Scan">
        </div>
        <span>Scan</span>
      </div>
    </div>


    <!--SHOW ONLY ON TABLET OR LARGER-->
    <div class="section-container show-tablet">
      <h1>Product Markets</h1>

        <div class="markets-container">
          <a href="#">
            <div class="markets-wrapper drop-shadow">
              <img src="img/datacomm.png" alt="Data Comm">
              <p><strong>DataComm</strong></p>
            </div>
          </a>

          <a href="#">
            <div class="markets-wrapper drop-shadow">
              <img src="img/hvac.png" alt="HVAC">
              <p><strong>HVAC</strong></p>
            </div>
          </a>

          <a href="#">
            <div class="markets-wrapper drop-shadow">
              <img src="img/industrial.png" alt="Industrial">
              <p><strong>Industrial</strong></p>
            </div>
          </a>

          <a href="#">
            <div class="markets-wrapper drop-shadow">
              <img src="img/lighting.png" alt="Lighting">
              <p><strong>Lighting</strong></p>
            </div>
          </a>

          <a href="#">
            <div class="markets-wrapper drop-shadow">
              <img src="img/energy.png" alt="Energy Efficiency">
              <p><strong>Energy Efficiency</strong></p>
            </div>
          </a>

          <a href="#">
            <div class="markets-wrapper drop-shadow">
              <img src="img/utility.png" alt="Utility">
              <p><strong>Utility</strong></p>
            </div>
          </a>

        </div> <!--Markets Container Close-->
    </div> <!--Section Container Close-->

    <div class="front-page-info-elements-container">
      <div class="front-page-info-element-deal-wrapper section-container drop-shadow">
        <img class="img-responsive" src="panel/deal.png" alt="Click for deals!">
      </div>

      <div class="front-page-info-element-member-wrapper section-container drop-shadow">
        <img class="img-responsive" src="img/platt_plus.png" alt="Get Plat Plus!">
        <h2>Get Started Today</h2>
        <h3>Become a <span>Platt Plus</span> Member.</h3>
        <a class="button-oval-link" href="#">Learn More</a>
      </div>

      <div class="front-page-info-element-recent-wrapper section-container drop-shadow">
        <!--TODO Dynamic Vue Component-->
        <span class="recent-title">Recently Viewed</span>
        <span>View All</span>

        <img class="img-responsive" src="recent/11.png" alt="Product ID 11">
        <img class="img-responsive" src="recent/22.png" alt="Product ID 22">
        <img class="img-responsive" src="recent/22.png" alt="Product ID 22">
      </div>
    </div> <!--Front Page Info Elements Container-->

    <div class="front-page-info-element-squares-container section-container">
      <div class="front-page-info-element-square-wrapper">
        <div class="front-page-info-element-square">
          <img src="" alt="">
        </div>
      </div>

      <div class="front-page-info-element-square">test</div>
      <div class="front-page-info-element-square">test</div>
      <div class="front-page-info-element-square">test</div>
    </div>



  </div>
</template>

<script>

export default {
  name: 'app',
  components: {

  }
}
</script>
