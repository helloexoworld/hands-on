---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
title: 'Step 2.3: Load time series raw data'
category: step-2
before: 'step-2-Keplers-Data/2.2-Exploring-known-time-series'
next: 'step-2-Keplers-Data/2.4-Split-Kepler-11-data'
back: 'step-2-Keplers-Data/2.3-Getting-Kepler-11-raw-data'
---

## Solutions

<warp10-embeddable-quantum warpscript="
// Storing the token into a variable
@HELLOEXOWORLD/GETREADTOKEN 'token' STORE 

// FETCH
[ 
    $token                              // Application authentication
    'sap.flux'                          // selector for classname
    { 'KEPLERID' '6541920' }            // Selector for labels
    '2009-05-02T00:56:10.000000Z'       // Start date
    '2013-05-11T12:02:06.000000Z'       // End date
] 
FETCH
">
</warp10-embeddable-quantum>