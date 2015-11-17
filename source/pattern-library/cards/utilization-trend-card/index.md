---
title: Utilization Trend Card
author: rhamilto
layout: page
---
<div>
  {% include nav-tabs-pattern.html %}
  <div class="tab-content">
    <div role="tabpanel" class="tab-pane active" id="overview">
      <p>Utilization cards display the current utilization and a trend of a single metric.  The most common use case for this pattern is seen in a dashboard.</p>
      <h3>Card with a Single Metric</h3>
      <!-- don't copy this example as it's been modified to work within the context of the documentation -->
      <div class="cards-pf">
        <div class="container-fluid container-cards-pf" style="margin-top: 0;">
          <div class="row row-cards-pf" style="padding-top: 20px;">
            <!-- Important:  if you need to nest additional .row within a .row.row-cards-pf, do *not* use .row-cards-pf on the nested .row  -->
            {% include card-pf-utilization-single-metric.html chart1="chart-pf-donut" chart2="chart-pf-sparkline" %}
          </div>
        </div>
      </div>
      <h3>Card with Multiple Metrics</h3>
      <!-- don't copy this example as it's been modified to work within the context of the documentation -->
      <div class="cards-pf">
        <div class="container-fluid container-cards-pf" style="margin-top: 0;">
          <div class="row row-cards-pf" style="padding-top: 20px;">
            <!-- Important:  if you need to nest additional .row within a .row.row-cards-pf, do *not* use .row-cards-pf on the nested .row  -->
            {% include card-pf-utilization-multiple-metrics.html chart3="chart-pf-donut-2" chart4="chart-pf-sparkline-2" chart5="chart-pf-donut-3" chart6="chart-pf-sparkline-3" chart7="chart-pf-donut-4" chart8="chart-pf-sparkline-4" %}
          </div>
        </div>
      </div>
    </div>
    <div role="tabpanel" class="tab-pane" id="design">
      <h3>Card with a Single Metric</h3>
      <div class="row">
        <div class="col-md-7">
          <img src="/wp-content/uploads/2015/08/singe-metric-utilization-card2.png" alt="singe-metric-utilization-card2" />
        </div>
        <div class="col-md-5">
          <ol>
            <li><b>Metric Title:</b> Display the metric name.</li>
            <li><b>Current Value:</b> Display the current value. This could be available, which is the PatternFly default, or used.</li>
            <li><b>Label:</b> The label for the value is left aligned and listed above the total value.</li>
            <li><b>Total Value:</b> The total value is left aligned and listed under the label.</li>
            <li><b>Unit of Measurement:</b> The label for unit of measurement is shown after the total value.</li>
            <li><b>Content Separator:</b> A horizontal line visually separates the content in the card. The content separator is located below the values and above the donut chart. </li>
            <li><b>Donut Chart:</b> See the <a href="/patterns/donut-chart/">Donut Chart Pattern</a> for more details.</li>
            <li><b>Sparkline:</b> See the <a href="/patterns/sparkline/">Sparkline Pattern</a> for more details.</li>
            <li><b>Time Frame:</b> The time frame is indicated under the sparkline by small text and is left aligned.</li>
          </ol>
        </div>
      </div>
      <h3>Card with Multiple Metrics</h3>
      <div class="row">
        <div class="col-md-7">
          <img src="/wp-content/uploads/2015/08/multi-metric-utilization-card-callout1.png" alt="multi-metric-utilization-card-callout"/>
        </div>
        <div class="col-md-5">
          <ol>
            <li><b>Card Title:</b> Use a card title if multiple metrics are shown in one card.</li>
            <li><b>Title Separator:</b> Include a horizontal line under the card title.</li>
            <li><b>Metric Title:</b> Display the metric name.</li>
            <li><b>Current Value:</b> Display the current value. This could be available, which is the PatternFly default, or used.</li>
            <li><b>Label:</b> The label for the value is left aligned and listed above the total value.</li>
            <li><b>Total Value:</b> The total value is left aligned and listed under the label.</li>
            <li><b>Unit of Measurement:</b> The label for unit of measurement is shown after the total value.</li>
            <li><b>Content Separator:</b> A horizontal line visually separates the content in the card. The content separator is located below the values and above the donut chart.</li>
            <li><b>Donut Chart:</b> See the <a href="/patterns/donut-chart/">Donut Chart Pattern</a> for more details.</li>
            <li><b>Sparkline:</b> See the <a href="/patterns/sparkline/">Sparkline Pattern</a> for more details.</li>
            <li><b>Time Frame:</b> The time frame is indicated under the sparkline by small text and is left aligned.</li>
          </ol>
        </div>
      </div>
    </div>
    <div role="tabpanel" class="tab-pane" id="code">
      {% include nav-tabs-code.html %}
      <div class="tab-content">
        <div role="tabpanel" class="tab-pane nested active" id="ref-impl">
          <h3>Card with a Single Metric</h3>
          <div class="example-pf">
            <div class="cards-pf">
              <div class="container-fluid container-cards-pf" style="margin-top: 0;">
                <div class="row row-cards-pf" style="padding-top: 20px;">
                  <!-- Important:  if you need to nest additional .row within a .row.row-cards-pf, do *not* use .row-cards-pf on the nested .row  -->
                  {% include card-pf-utilization-single-metric.html chart1="chart-pf-donut-5" chart2="chart-pf-sparkline-5" %}
                </div>
              </div>
            </div>
          </div>
          <button class="btn btn-default btn-copy">Copy</button>
          <pre class="prettyprint">{% capture markup_include %}{% include card-pf-utilization-single-metric.html chart1="chart-pf-donut-5" chart2="chart-pf-sparkline-5" %}{% endcapture %}{{ markup_include | xml_escape }}</pre>
          <h3>Card with Multiple Metrics</h3>
          <div class="example-pf">
            <!-- don't copy this example as it's been modified to work within the context of the documentation -->
            <div class="cards-pf">
              <div class="container-fluid container-cards-pf" style="margin-top: 0;">
                <div class="row row-cards-pf" style="padding-top: 20px;">
                  <!-- Important:  if you need to nest additional .row within a .row.row-cards-pf, do *not* use .row-cards-pf on the nested .row  -->
                  {% include card-pf-utilization-multiple-metrics.html chart3="chart-pf-donut-6" chart4="chart-pf-sparkline-6" chart5="chart-pf-donut-7" chart6="chart-pf-sparkline-7" chart7="chart-pf-donut-8" chart8="chart-pf-sparkline-8" %}
                </div>
              </div>
            </div>
          </div>
          <button class="btn btn-default btn-copy">Copy</button>
          <pre class="prettyprint">{% capture markup_include %}{% include card-pf-utilization-multiple-metrics.html chart3="chart-pf-donut-6" chart4="chart-pf-sparkline-6" chart5="chart-pf-donut-7" chart6="chart-pf-sparkline-7" chart7="chart-pf-donut-8" chart8="chart-pf-sparkline-8" %}{% endcapture %}{{ markup_include | xml_escape }}</pre>
        </div>
        <div role="tabpanel" class="tab-pane nested" id="angular">
          [angular code goes here]
        </div>
      </div>
    </div>
    <div role="tabpanel" class="tab-pane" id="usability-test">
      [ usability content goes here ]
    </div>
  </div>
</div>