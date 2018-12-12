---
title: "Progress"
author: "Stephanie"
date: "5 November 2018"
output: html_document
---

## MAY

Administration

## JUNE 

1. Hexmap algorithm
    Plan inputs, outputs, functions and structure of sub-functions:
    (a)  read in polygons
    (a)  create a hexagon grid, user specified size
        - add a user specified buffer around geography of centroids
        
    (a)  calculate how far each polygon centroid is from capital cities
    (a)  assigning each polygon to a spot on the hexagon grid map
        - filter grid for close, available grid points
        - pick the closest

1. Began writing code for:
    - grid creation
    - grid filtering to consider the angle from closest city to centroid, use this to only consider grid points that fall within range around that angle 
    - finding distance between centroid and available grid points

## JULY

1. Began writing code for:
    - finding the closest capital city
    - reordered allocation of hexagons, ascending distance from closest capital city
    
A. useR!2018 Conference                                    
A. FIT9133: Programming fundamentals in Python: Semester 2, Monash University 

1. Attempt smoothing null data to contrast to spatially distributed data

## AUGUST

1. Read in sf object
    - ensure no null geometries
    - project data in Australian standard projection
    - automate deriving bbox and hexagon size
    - derive centroids from projected polygons
    


##  SEPTEMBER

1. *Tidy to allow provision of polygons*
1. Created SugaRbag package; to organise and document functions that implement the hexmap algorithm
    - include capital cities as a data set
    - included simplified data for SA2 in 2011 and 2016
    - allowed data to be provided as Rda or ESRI
    - create projected long lat centroids tibble 
    - improved bbox creation using centroids tibble


##  OCTOBER

1. *Automate tuning for size of hexagons*
1. Improving SugaRbag package;
    - created function to filter grid points, ensures at least one point is returned
    - column included to identify each polygon
    - implemented algebraic method to filter grid for a 60 degree slice of a circle around centroid
    - allow users to provide their own focal points
    - allocate all in one function call
    - check buffer distance is appropriate
    - vastly improved buffer grid, rolling average minimum and maximum of the centroids in Australian border
    - created a sandbox for easier testing and implementation of changes

A. Completed exam for FIT9133

##  NOVEMBER


1. Create a main function to call others
    - Provide output as a list of two, the hexmap allocations and tibble with geometry column
    - allow shape files in environment to be provided
    - show user the prgoression through steps
    - create facetted maps using geofacet
    - create plots of geography and hexagons
    - turn hexagon centroids into hexagon polygons
    - enhance use of subsets of shape files
    - Queensland vingette
    - Spatial distributions of cancer vignette
    
## DECEMBER

1. Secured LGA data for TIA in Victoria
    - isolated issues created when sf_id is not unique
    - built check for unique ID
    - LGA vignette for Victoria
    

1. *Prepare thesis chapter for submission*
    - began structure of thesis chapter

##  JANUARY - FEBRUARY

2. *Preparation of survey questions*

## MARCH

A. *ETC4541: Bayesian time series econometrics: Semester 1, Monash University*

## APRIL 

A. *Annual Progress Report*                         

## MAY

2. *Execution of experiment*              
2. *Data Analysis*                

## JUNE

2. *Data Analysis*  
A. *Complete exam for ETC4541*

## JULY

A. *Prepare thesis chapter for submission* 

## AUGUST - SEPTEMBER

3. *Apply transformation algorithm, polygons to hexagons*

## OCTOBER

3. *Prepare thesis chapter for submission*               

## NOVEMBER

A. *Complete masters thesis*                             
