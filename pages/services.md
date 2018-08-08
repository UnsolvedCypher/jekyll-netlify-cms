---
title: Solutions
permalink: /solutions
layout: default
heading: Our Solutions
subheading: We have a variety of solutions to meet your needs
bg-class: bg-3
extra_head: |
  <link href="//cdn.rawgit.com/noelboss/featherlight/1.7.13/release/featherlight.min.css" type="text/css" rel="stylesheet" />
  <link href="//cdn.rawgit.com/noelboss/featherlight/1.7.13/release/featherlight.gallery.min.css" type="text/css" rel="stylesheet" />
extra_script: |
  <script src="//cdn.rawgit.com/noelboss/featherlight/1.7.13/release/featherlight.min.js" type="text/javascript" charset="utf-8"></script>
  <script src="//cdn.rawgit.com/noelboss/featherlight/1.7.13/release/featherlight.gallery.min.js" type="text/javascript" charset="utf-8"></script>

---

<!-- Portfolio Start -->
<div class="container">

  <h2><strong>B2B Fulfillment Products/Services</strong></h2>
  <section>
    <div class="row">
      <div class="col-md-4">
        <h3>Full Service Fulfillment</h3>
        <p>Our traditional fulfillment services combine time-honored publishing solutions with unparalleled customer service.  Early in the onboarding process, a dedicated Account Manager is assigned to your account.  They are responsible for processing of every publication issue and take the lead on other services identified and customized to your fulfillment needs.  Online subscription centers with registration authentication and full audit preparation are but a few of the of services/solutions available.</p>
      </div>

      <div class="col-md-4">
        <h3>E-Circ</h3>
        <p>E-Circ is CFs online tool that allows our traditional fulfillment customers access to their circulation database(s).  Here, you can run counts on any field(s) within the circulation database and export data based on your query results.  There is also a look up function which provides current information on your subscribers for customer inquiries.</p>
      </div>
      <div class="col-md-4">
        <h3>CircView</h3>
        <p>CircView is our self-service fulfillment solution primarily for paid products, offering a full range of financial reporting options.  CircView enables you to perform your own customer and order entry and issue processing.  CircView supports group/site licenses, various subscription levels, trial promotions, pay-per article and can be integrated with Authorize.net or PayPal payment gateway accounts. </p>
    </div>
    </div>

    <h2><strong>Integrated Database Products</strong></h2>
    <div class="row">
      <div class="col-md-4">
        <h3>MediaView</h3>
        <p>MediaView is our proprietary audience management solution, created, supported and by our in-house team of developers.  MediaView was developed to meet the pressing need expressed by so many publishers to turn disparate multichannel customer data into actionable intelligence by giving publishers the power to:
          <ul>
            <li>Identify users of one product that may be ideal prospects for another</li>
            <li>Develop highly targeted audience segments and implement real “one-to-some” marketing</li>
            <li>Launch aggressive cross-sell strategies based on multichannel audience intelligence</li>
            <li>Build audience profiles and lists to drive product extensions and new product developments</li>
            <li>Realize operational savings by automating data handling tasks</li>
            <li>Produce higher data quality</li>
        </ul></p>
      </div>
      <!-- <div class="col-md-4">
        <h3>MediaView Lite</h3>
        <p>This is our newest web based, self-service integrated database solution.  It was developed as a solution for smaller publishers to harness the power of MediaView at a lower cost. There are limitations on number of brands and users.  Most of the same modules available in MediaView are also available in MV Lite.  The Web Analytics Manager functionality is not available with this product.</p>
    </div> -->
      <div class="col-md-4">
        <h3>CF API</h3>
        <p>CF has a series API services that allow you to access and add to the your database housed at CF. There are services for the following:<ul>
            <li>Add a record for those clients who prefer to host/manage their own online subscription forms</li>
            <li>Retreive all records changed within a time period</li>
            <li>Lookup subscribers based on email or account number</li>
            <li>Validate active subscribers for authentication (website registration/iPad)</li>
          </ul>
        For more information, please contact info@computerfulfillment.com</p>
      </div>
      <div class="col-md-4">
        <img src="images/folio.png" alt="Folio" class="folio-image" />
      </div>
    </div>
    <br />
    <br />
    <br />
    <!-- <hr /> -->
    <!-- <h3>MediaView</h3>
    <p>Stuff about MediaView etc etc etc</p>
    <h3>CircView</h3>
    <p>Stuff about CircView etc etc etc</p>
    <h3>OtherView</h3>
    <p>More stuf etc etc etc</p> -->
  </section>
  <h2>Gallery</h2>
  <p>Click on an item to learn more</p>
  <hr />
  <section data-featherlight-gallery data-featherlight-filter="a">
  {% for item in site.data.solutions_gallery %}
  {% cycle '<div class="row">', '', '' %}
    <div class="col-md-4">
      <div class="overlay-container">
        <a href="#" data-featherlight="<h2>{{ item.title }}</h2><img src='images/solutions-gallery/{{ item.image }}' /><br /><p>{{ item.description }}</p>">
          <img src="images/solutions-gallery/{{ item.image }}" width="90%">
          <div class="middle"><h2>{{ item.title }}</h2></div>
        </a>
      </div>
    </div>
  {% cycle '', '', '</div>' %}
  {% endfor %}

  {% assign mod_val = site.data.solutions_gallery | size | modulo: 3 %}
  {% for i in (1..mod_val) %}
    <div class="col-md-4"></div>
  {% endfor %}

  {% if mod_val > 0 %}
    </div>
  {% endif %}
</section>
</div>

<!-- <script src="script.js"> -->
