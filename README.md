# Infotrack-technical-test-automation-suite
<H1>API test suite</H1>
<p>This Test Suite is used for Testing and Validating ENDPOINTS for the following base url:
https://reqres.in/
<br>
<H2>TEST SUITE HIGH LEVEL BREAKDOWN</H2></p>
<strong>- NOTE: Please refer to each subsections for detailed test Overview and description </strong>
<br>
<H3>FUNCTIONAL TESTS</H3>
<H4>BEARER TOKEN VALUE TEST</H4>
<p>Tests to obtain and Submit a bearer token to multiple endpoints (GET,POST,PUT,DELETE)</p>
<H4>NEGATIVE TESTS</H4>
<i>Used to Test Negative scenarios where input of invalid or incorrect data, etc are used to test expected error handling and responses from the API endpoint and/or response contents.</i>
<H4>E2E TESTS</H4>
<p>Used to test E2E Flows Scenarios</p>
<H4>API PERFORMANCE TESTS - SAMPLE</H4>
<i>API Performance Test: These sample Tests are used to validate response times on the Endpoints and to create a base suite that can be shared with other Performance Tools e.g Gattling, Jmeter,K6(load Testing - peak metrics - endurance tests)</i>
<H4>TEST REPORTS</H4>
<p>Using <strong>htmlextra</strong> npm library for Newman or Postman Runner Test Run Snippets where not available</p>
<br>

<H2>INSTRUCTIONS AND USAGE</H2>
<H3><strong>HOW TO RUN:</strong></H3>
<p>Download Postman Client via web browser or via Node Package Manager</p> 
https://www.postman.com/
https://www.npmjs.com/get-npm
<p>Download Newman to run the collection suite via Command Line Interface or Terminal using the following Node Package Manager command</p>
<i>npm install -g newman</i>
<p>*Please verify you are using the latest version of NPM and POSTMAN for compatibility.</p>
<H4>TEST REPORTING USING HTMLEXTRA Reports</H4>
<p>This is a Newman HTML reporter that has been extended to include the separation of the iteration runs so these are no longer aggregated together and also some additional handlebars helpers to enable users to create better custom templates<p>
https://www.npmjs.com/package/newman-reporter-htmlextra
 <br>
to install htmlextra use the following Node Package Manager command after installing Npm & Newman (see below)</p>
<i>npm install -g newman-reporter-htmlextra</i>
<H5>GENERATING HTML REPORTS</H5>
 <p>run the following command to use the library (which specifies the Collection and environment and reporter to use)</p>
<strong><i>newman run infotrack_technical_test.postman_collection.json -e reqres_in_postman_environment.json -r htmlextra</i></strong>
<br>
<p>*Please verify you are inside the correct folder location and both files exactly match the file names in the command</p>
<footer>
<p><i>Created by Harold Baldwin (github: sirhazman07)
 on 15/05/2017<p><i>
<p>This source code (collection and environment files hosted in github 
<a href= "https://github.com/sirhazman07/Infotrack-technical-test-automation-suite">here</a>
</p>
</footer>
