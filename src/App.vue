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
            <a href="#search"><img class="icon icon-white-search" src="img/ic/white/ic_search.png" alt="Search"></a>
          </li>
          <li>
            <a href="#search"><img class="icon icon-white-shopping-cart" src="img/ic/white/ic_shopping_cart.png" alt="Shopping Cart"></a>
          </li>
          <li>
            <a href="#search"><img class="icon icon-white-person" src="img/ic/white/ic_person.png" alt="Profile"></a>
          </li>
          <li>
            <a href="#search"><img class="icon icon-white-menu" src="img/ic/white/ic_menu.png" alt="Menu"></a>
          </li>
        </ul>
      </div>

      <div class="search-wrapper">
        <search />
      </div>

    </header><!--header-->


    <div id="categories-wrapper" class="categories-wrapper">
      <!--TODO - Make category containers vue components-->
      <!--TODO - Spacing and borders - Might need it to be a sub grid element to line up the right way-->

      <div class="categories-element categories-element-all">
        <img src="img/ic/black/ic_categories.png" alt="All Categories Icon">
        <strong><h2>Shop all categories</h2></strong>
        <img class="categories-element-arrow" src="img/ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="img/ic/black/ic_playlist_add_check.png" alt="My Catalog Icon">
        <h3>My Catalog</h3>
        <img class="categories-element-arrow" src="img/ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="img/ic/black/ic_list.png" alt="My List Icon">
        <h3>My List</h3>
        <img class="categories-element-arrow" src="img/ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="img/ic/green/ic_chat_active.png" alt="Chat Active Icon">
        <h3>Live Help</h3>
        <img class="categories-element-arrow" src="img/ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="img/ic/black/ic_check_circle.png" alt="PIM">
        <h3>PIM</h3>
        <img class="categories-element-arrow" src="img/ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="img/ic/black/ic_playlist_add_check.png" alt="Account Icon">
        <h3>Account</h3>
        <img class="categories-element-arrow" src="img/ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>

      <div class="categories-element">
        <img src="img/ic/black/ic_place.png" alt="Branch Locations">
        <h3>Branch Locations</h3>
        <img class="categories-element-arrow" src="img/ic/black/ic_arrow_forward.png" alt="Go to all categories">
      </div>
    </div> <!--categories-wrapper-->


    <!--SHOW ONLY ON MOBILE-->
    <div class="section-container functionality-circle-container show-phone">
      <!--TODO - Make these components-->
      <div class="functionality-circle-wrapper">
        <div class="functionality-circle drop-shadow">
          <img src="img/ic/green/ic_line_style.png" alt="Categories">
        </div>
        <span>Categories</span>
      </div>

      <div class="functionality-circle-wrapper">
        <div class="functionality-circle drop-shadow">
          <img src="img/ic/green/ic_search.png" alt="Search">
        </div>
        <span>Search</span>
      </div>

      <div class="functionality-circle-wrapper">
        <div class="functionality-circle drop-shadow">
          <img src="img/ic/green/ic_scanner.png" alt="Scan">
        </div>
        <span>Scan</span>
      </div>
    </div> <!--functionality-circle-container-->


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

        </div> <!--markets-container-->
    </div> <!--section-container-->


    <div class="front-page-info-elements-container">
      <div class="front-page-info-element-deal-wrapper section-container drop-shadow">
      </div>

      <div class="front-page-info-element-member-wrapper section-container drop-shadow">
        <img class="" src="img/platt_plus.png" alt="Get Plat Plus!">
        <div class="front-page-info-element-member-copy">
          <h2>Get Started Today</h2>
          <h3>Become a <span>Platt Plus</span> Member.</h3>
          <br>
          <br>
          <br>
          <a class="button-oval-link" href="#">Learn More</a>
        </div>
      </div>

      <div class="front-page-info-element-recent-wrapper section-container drop-shadow">
        <!--TODO Dynamic Vue Component-->
        <span class="recent-title">Recently Viewed</span>
        <span>View All</span>

        <img class="img-responsive" src="img/recent/11.png" alt="Product ID 11">
        <img class="img-responsive" src="img/recent/22.png" alt="Product ID 22">
        <img class="img-responsive" src="img/recent/22.png" alt="Product ID 22">
      </div>
    </div> <!--front-page-info-elements-container-->


    <div class="front-page-info-element-squares-container section-container">
      <div class="front-page-info-element-square-wrapper drop-shadow">
        <div class="front-page-info-element-square">
          <img class="img-responsive" src="img/super_tool_day.png" alt="Super Tool Day">
          <p>Super Tool Day & Dynamic Data Day</p>
        </div>
      </div>

      <div class="front-page-info-element-square-wrapper drop-shadow">
        <div class="front-page-info-element-square">
          <img class="img-responsive" src="img/ic_location_b.png" alt="Branch Locations">
          <p>Branch Locations</p>
        </div>
      </div>

      <div class="front-page-info-element-square-wrapper drop-shadow">
        <div class="front-page-info-element-square">
          <img class="img-responsive" src="img/ic_helpcenter.png" alt="Help Center">
          <p>Help Center</p>
        </div>
      </div>

      <div class="front-page-info-element-square-wrapper drop-shadow">
        <div class="front-page-info-element-square">
          <img class="img-responsive" src="img/ic_platt-u.png" alt="Platt U">
          <p>Platt U</p>
        </div>
      </div>
    </div> <!--front-page-info-element-squares-container -->


    <div class="front-page-info-element-app-container section-container drop-shadow">
      <div class="front-page-info-element-app-image"></div>
      <div class="front-page-info-element-app-copy">
        <span>Shop better, download the Platt App today</span>
      </div>
    </div><!--front-page-info-element-app-container-->


    <footer>
      <!--TODO - Clean this up-->
      <a href="#"><h2>Support Center</h2></a>

      <h2>800-25-Platt</h2>
      <span>800-257-5288</span>
      <br>
      <br>
      <br>
      <h2 class="footer-phone-time">4 a.m. - 12 a.m. (pst)</h2>
      <h2 class="footer-phone-time">7 Days a week</h2>
      <br>
      <br>
      <br>
      <a class="button-oval-link" href="#">
        <img class="button-icon" src="img/ic/black/ic_chat.png" alt=""><span style="color: black">Live Help</span>
      </a>
      <br>
      <br>

      <div class="footer-nav show-tablet">
          <a href="#"><h3>Contact Us</h3></a>
          <a href="#"><h3>What's New</h3></a>
          <a href="#"><h3>FAQ's</h3></a>
      </div>
    </footer>

  </div>
</template>

<script>
import Search from './components/Search';
export default {
  name: 'app',
  components: {
    Search
  }
}
</script>
