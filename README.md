<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>Citrix NetScaler Monitoring Plugin</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <meta http-equiv="X-UA-Compatible" content="IE=EmulateIE8" />
    <meta content="Scroll Wiki Publisher" name="generator"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/liquid.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/print.css" media="print"/>
    <link type="text/css" rel="stylesheet" href="css/content-style.css" media="screen, projection, print"/>
    <link type="text/css" rel="stylesheet" href="css/screen.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/print.css" media="print"/>
</head>
<body>
                <h1>Citrix NetScaler Monitoring Plugin</h1>
    <div class="section-2"  id="174462535_CitrixNetScalerMonitoringPlugin-Overview"  >
        <h2>Overview</h2>
    <p>
    </p>
    <p>
            <img src="images_community/download/attachments/174462535/icon.png" alt="images_community/download/attachments/174462535/icon.png" class="confluence-embedded-image" />
        Retrieve statistics from a Citrix NetScaler service using the NITRO API    </p>
    <div class="tablewrap">
        <table>
<thead class=" "></thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Name and Version    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Citrix NetScaler Monitoring Plugin    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Compatible with    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
5.6 / 6.0    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Author    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Roman Spitzbart (roman.spitzbart@compuware.com)    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/Licenses">License</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_5275722_2_dynaTraceBSD.txt">dynaTrace BSD</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/Support+Levels">Support Level</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/Support+Levels">Not Supported</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Download    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_174752373_1_com.compuwareapm.dynatrace.plugin.netscaler_1.0.0.jar">NetScaler Monitoring Plugin 1.0.0</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Description    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Retrieve statistics from a Citrix NetScaler services through the NITRO API    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Release History    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
2014-07-28 Initial release    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    <p>
    <span style="color: #505050;">
<br/>    </span>
    </p>
    <p>
    <span style="color: #505050;">
Installation    </span>
    </p>
    <p>
Import the Plugin into the dynaTrace Server via the &quot;Settings&quot; - &quot;dynaTrace Server&quot; menu -&gt; &quot;Plugins&quot; -&gt; &quot;Install Plugin&quot;. For details how to do this please refer to the <a href="https://community.compuwareapm.com/community/display/DOCDT60/Plugin+Management">dynaTrace documentation</a>.    </p>
    </div>
    <div class="section-2"  id="174462535_CitrixNetScalerMonitoringPlugin-Usage"  >
        <h2>Usage</h2>
    <p>
The plugin has 5 required parameters:    </p>
    <div class="tablewrap">
        <table>
<thead class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
<strong class=" ">Parameter</strong>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Description    </p>
            </td>
        </tr>
</thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Service    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Name of the Citrix NetScaler service to query    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
URI    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
URI of the NITRO API REST web service (see <a href="http://support.citrix.com/proddocs/topic/netscaler-main-api-10-1-map/ns-nitro-rest-feat-stat-api-ref.html">here </a>for details) / default is &quot;/nitro/v1/stat/service&quot;    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Port    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Port for the NITRO API REST web service / default ist 80    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Username    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Password    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    <p>
If you want to query more than one service configure multiple monitors with the different service names!    </p>
    <p>
The following measures are returned by the plugin:    </p>
    <div class="tablewrap">
        <table>
<thead class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Measure    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Description    </p>
            </td>
        </tr>
</thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
State    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
0 - service down/out of service    </p>
    <p>
1 - service up    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Average TTFB    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Average Time-to-first-byte in ms    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Response Rates    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Current Client Connections    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Current Server Connections    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    <p>
Each measure is split by the service name - make sure you select the correct splitting.    </p>
    </div>
    <div class="section-2"  id="174462535_CitrixNetScalerMonitoringPlugin-Screenshots"  >
        <h2>Screenshots</h2>
    <p>
            <img src="images_community/download/attachments/174462535/netscaler_monitor_config.png" alt="images_community/download/attachments/174462535/netscaler_monitor_config.png" class="confluence-embedded-image" />
            </p>
    <p>
            <img src="images_community/download/attachments/174462535/netscaler_monitor_measures.png" alt="images_community/download/attachments/174462535/netscaler_monitor_measures.png" class="confluence-embedded-image" />
            </p>
    <p>
            <img src="images_community/download/attachments/174462535/netscaler_monitor_measures_2.png" alt="images_community/download/attachments/174462535/netscaler_monitor_measures_2.png" class="confluence-embedded-image" />
            </p>
    </div>
            </div>
        </div>
        <div class="footer">
        </div>
    </div>
</body>
</html>
