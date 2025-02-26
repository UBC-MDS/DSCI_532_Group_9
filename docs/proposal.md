Proposal
================

## Motivation and purpose

Our role: Data scientist consultancy firm

Target audience: Agricultural practitioners, Beekeepers/Apiarists

Bees are one of the most essential components of modern agriculture.
Most plants need to be pollinated by animal visitors, especially
insects. A wide variety of flowering plants, such as the everyday
visible fruits like apples and blueberries, require managed pollinators
to be able to ensure production. Honey bees are ideal for pollination
because they are easy to move and manage. However, during the winter of
2006-2007, some beekeepers in America began to report unusually high
losses of 30-90 percent of their hives. Colony loss has declined since
then but is still a concern. Since the number of bee colonies is closely
related to agricultural production, there is a need for agricultural
decision-makers and practitioners to know the status of local bee
colonies, especially the number, loss trend, and colony stressors.

To meet the needs of agricultural development, we decided to build a
data visualization app with open data to ensure that agricultural
practitioners can explore bee colony data visually. Our application will
display the number of bee colonies in each state of the United States
over the years and allow users to explore changes in colony numbers and
colony stressors by filtering by state and time.

## Description of the data

The honey bee colonies and stressors dataset were obtained from
[TidyTuesday](https://github.com/rfordatascience/tidytuesday/blob/master/data/2022/2022-01-11/readme.md)
who in turn obtained the raw data from the United States Department of
Agriculture (USDA).

The USDA collected the time series data from a stratified sample of
operations across the United States that responded as having bees on the
Bee and Honey Inquiry, and from the National Agriculture Statistics
Service list frame. Data was collected on a quarterly basis for
operations with five or more colonies, and on an annual basis for
operations with less than five colonies.

In our dashboard, we will visualize `colony_max` and `colony_loss_pct`
on a geographic map of the United States. The variables `colony_max` and
`colony_loss_pct` are the maximum number of colonies in a state for a
particular time period, and the number of lost colonies since the start
of the time period divided by `colony_max`, respectively. We will also
visualize `colony_n`, the number of colonies in a state, as a time
series plot. Our final visualization will be the percentage of colonies,
`stress_pct`, that are affected by different colony health stressors,
`stressor`, for a particular state over time as a stacked bar plot.

## Research questions and usage scenarios

Our project, the `Bee Colony Dashboard` helps identify the rate and
possible causes of colony collapse disorder over quarterly periods in
the US. Some key questions that can be answered are:

1.  Which state has the highest/lowest colony loss percentage over time?

2.  What are possible causes of colony collapse disorder?

3.  What specific problems do certain state’s colonies face over time?

Below is a usage scenario of our dashboard:

Buzzing Bee is a beekeeping company interested in researching colony
loss across the US. Since loss rates are high, the beekeepers are under
pressure to create new colonies to offset losses each year. The company
wants to work with agricultural practitioners and farms to keep their
bee colonies stable without the need to add new colonies each year.

John, is an apiarist working in Buzzing Bee and is assigned a project to
identify states where colony loss percentage is very high and to study
possible causes.

With the Bee Colony Dashboard, he will be able to identify bee colony
losses over quarterly periods in the US. The geographic map visual
illustrates how bee colony losses vary over each state for a single
period in time, and apiarists/beekeepers can gain an idea of the local
severity of colony stressors in different states. The time series plot
visualizes the number of colonies over time for a single state and will
inform apiarists/beekeepers of how problems affecting colonies
increase/decrease over time. The third visualization, the stacked bar
chart of stressors, gives insight on what specific problems a certain
state’s colonies face over time, and can provide crucial information on
what stressors need to be combatted to improve colony health.
