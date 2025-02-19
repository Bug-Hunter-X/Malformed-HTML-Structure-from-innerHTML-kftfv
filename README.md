# Malformed HTML Structure from innerHTML

This example demonstrates an uncommon HTML bug caused by incorrect usage of `innerHTML`.  The provided HTML code attempts to set the innerHTML of a div, but uses an improperly nested paragraph tag (<p>). This leads to unexpected behavior in rendering the page.

The solution shows how to correctly update the HTML using the DOM methods.  Avoid directly manipulating HTML with innerHTML when possible due to such potential issues.

## Bug:

The innerHTML assignment creates a malformed HTML string that the browser might handle differently depending on browser implementation, often silently ignoring the problem or producing unexpected results. 

## Solution:

The solution utilizes the DOM API to create a paragraph element correctly then inserts it into the DOM.