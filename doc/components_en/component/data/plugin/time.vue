<template>
  <div class="doc">
    <h2>TimePicker</h2>
    <h3>Basic</h3>
    <example demo="dataplugins/timepicker1"></example>

    <h3>Disabled</h3>
    <example demo="dataplugins/timepicker2"></example>

    <h3>Control selection range</h3>
    <example demo="dataplugins/timepicker3"></example>
    
    <h3>DatePicker Property</h3>
    <table class="table">
      <tr>
        <th>Property</th>
        <th>Description</th>
        <th>Type</th>
        <th>Optional</th>
        <th>Default</th>
      </tr>
      <tr>
        <td>disabled</td>
        <td></td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
      </tr>
      <tr>
        <td>type</td>
        <td>Types of component</td>
        <td>String</td>
        <td>date</td>
        <td>year, month, week, datetime, datehour</td>
      </tr>
      <tr>
        <td>option</td>
        <td>Configuration items, see the options below for details</td>
        <td>Object</td>
        <td>-</td>
        <td></td>
      </tr>
      <tr>
        <td>format</td>
        <td>Custom data format</td>
        <td>String</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>hasSeconds</td>
        <td>Whether to automatically format to second when selecting date and time</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
      </tr>
      <tr>
        <td>noBorder</td>
        <td>Whether there is a border, suitable for the drop-down selection of text</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
      </tr>
      <tr>
        <td>placeholder</td>
        <td>Show the default prompt</td>
        <td>String</td>
        <td>-</td>
        <td>please select</td>
      </tr>
      <tr>
        <td>startWeek</td>
        <td>When choosing a week, set the starting day of the week</td>
        <td>Number</td>
        <td>1, 2, 3, 4, 5, 6, 7</td>
        <td>Global Configuration <code>datepicker.startWeek</code>, For details, please go to <router-link to="/en/component/config">Global Configuration</router-link></td>
      </tr>
      <tr>
        <td>readonly</td>
        <td></td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
      </tr>
    </table>

    <h3>Option Property</h3>
    <table class="table">
      <tr>
        <th>Property</th>
        <th>Description</th>
        <th>Type</th>
        <th>Optional</th>
        <th>Default</th>
      </tr>
      <tr>
        <td>start</td>
        <td>Starting time</td>
        <td>Function, Object, String</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>end</td>
        <td>End Time</td>
        <td>Function, Object, String</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>disabled</td>
        <td>No date selectable</td>
        <td>Function</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>shortcuts</td>
        <td>Custom shortcuts</td>
        <td>[Object]</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>minuteStep</td>
        <td>Minute interval</td>
        <td>Number</td>
        <td>-</td>
        <td>5</td>
      </tr>
      <tr>
        <td>hours</td>
        <td>Custom optional hours</td>
        <td>Function</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>minutes</td>
        <td>Custom optional minutes	</td>
        <td>Function</td>
        <td>-</td>
        <td>-</td>
      </tr>
    </table>
  </div>
</template>