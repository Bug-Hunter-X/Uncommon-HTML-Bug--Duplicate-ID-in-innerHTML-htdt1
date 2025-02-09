# Uncommon HTML Bug: Duplicate ID in innerHTML

This repository demonstrates an uncommon HTML bug related to using `innerHTML` and creating duplicate IDs.  The bug arises when using `innerHTML` to inject HTML that contains an element with an ID that already exists in the DOM.  This can lead to unpredictable behavior and potential JavaScript errors.

## Bug Description

The primary issue lies in the use of `innerHTML` to insert a `<div>` with the id `myDiv` inside an existing `<div>` with the same ID. This creates a duplicate ID, violating HTML standards and potentially causing unexpected consequences.  While not directly causing a syntax error, it leads to problems when trying to access or manipulate the elements using their IDs.

## Solution

The solution involves avoiding the creation of duplicate IDs when using `innerHTML`.  Instead, focus on inserting content without duplicating existing IDs.  Alternatively, use DOM manipulation methods that work directly with the DOM structure, avoiding the possible pitfalls of `innerHTML`.