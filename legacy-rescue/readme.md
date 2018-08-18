# Overview

## Current Functionality 

The application you have been asked to enhance allows an agronomist to view
growth progress for the farmer they work with. The agronomist is responsible
for ensuring the farmer's fields produce the maximum amount of yield. In return for
the agronomist's efforts he is paid a percentage of the profits.

The farmer is allowed to specify the amount of growth they expect to see during 
each phase of the growing season. The farmer and the agronomist also track activities 
that need to occur during the growing season.

## Desired Enhancements

The agronomist has asked that the application be enhanced to allow him to work with more 
than one farmer. 

The agronomist would also like to specify which phase of the growing season each farmer should
perform their activities. 

The agronomist wants 

# Terms

## Growing Season

The growing season is broken up into three phases
 - Planning
 - Planting
 - Harvest

## Activity

Some kind of activity performed in the fields. The activities in this application are

 - Tilling
 - Crop Plan
 - Field Designation
 - Soil Sampling
 - Planting
 - Herbicide
 - Insecticide
 - Fertilizer
 - Observation
 - Detasseling
 - Harvesting
 - Storage
 - Sale
 

Each activity has varying statuses associated. The statuses for each activity is listed below.

 - Tilling: Planned, Done
 - Crop Plan: Submitted, Approved, Rejected
 - Field Designation: Submitted, Approved, Rejected
 - Soil Sampling: Done
 - Planting: Done
 - Herbicide: Planned, Done
 - Insecticide: Planned, Done
 - Fertilizer: Planned, Done
 - Observation: Done
 - Detasseling: Planned, Done
 - Harvesting: Done
 - Storage: Done
 - Delivery: Done
 - Sale: Sold
 
# Features

## View Growth timeline for Farmer

### View Planning Growing Phase Activities

#### Story

As an agronomist <br />
I want to view all Planning activities sequentially <br />
So that I can ensure the farmer is setup well for Planting.

#### Tilling Scenarios

#### Scenario: Planned Tilling
Given I am working with one farmer <br/>
And we have planned tilling <br/>
When I view the farmer's timeline <br />
Then I should see the tilling activity in planned status <br />
And I should see tilling in the planning phase of the growing season

#### Scenario: Tilling Done
Given I am working with one farmer <br/>
And we have planned tilling <br/>
And we have finished tilling <br />
When I view the farmer's timeline <br />
Then I should see the tilling activity in done status <br />
And I should see tilling in the planning phase of the growing season

#### Crop Plan Scenarios

##### Scneario: Submitted Crop Plan
Given I am working with one farmer <br/>
And I have created a crop plan <br/>
When I view the farmer's timeline <br />
Then I should see the crop plan activity in submitted status <br />
And I should see the crop plan in the planning phase of the growing season

##### Scneario: Approved Crop Plan
Given I am working with one farmer <br />
And I have created a crop plan <br />
And the farmer has approved the crop plan <br />
When I view the farmer's timeline <br />
Then I should see the crop plan activity in approved status <br />
And I should see the crop plan in the planning phase of the growing season

##### Scneario: Rejected Crop Plan
Given I am working with one farmer <br />
And I have created a crop plan <br />
And the farmer has rejected the crop plan <br />
When I view the farmer's timeline <br />
Then I should see the crop plan activity in rejected status <br />
And I should see the crop plan in the planning phase of the growing season

##### Scneario: Resubmitted Crop Plan After Rejection
Given I am working with one farmer <br />
And I have created a crop plan <br />
And the farmer has rejected the crop plan <br />
And I have resubmitted the crop plan <br />
When I view the farmer's timeline <br />
Then I should see the crop plan activity in submitted status <br />
And I should see the crop plan in the planning phase of the growing season

#### Field Designation Scenarios

##### Scenario: Submitted Field Designation
Given I am working with one farmer <br />
And I have designated the farmer's fields <br />
When I view the farmer's timeline <br />
Then I should see the field designation activity in submitted status <br />
And I should see the field designation in the planning phase of the growing season

##### Scenario: Approved Field Designation
Given I am working with one farmer <br />
And I have designated the farmer's fields <br />
And the farmer has approved the field designation <br />
When I view the farmer's timeline <br />
Then I should see the field designation activity in approved status <br />
And I should see the field designation in the planning phase of the growing season

##### Scenario: Rejected Field Designation
Given I am working with one farmer <br />
And I have designated the farmer's fields <br />
And the farmer has rejected the field designation <br />
When I view the farmer's timeline <br />
Then I should see the field designation activity in rejected status <br />
And I should see the field designation in the planning phase of the growing season

##### Scenario: Resubmitted Field Designation After Rejection
Given I am working with one farmer <br />
And I have designated the farmer's fields <br />
And the farmer has rejected the field designation <br />
And I have resubmitted the field designation <br />
When I view the farmer's timeline <br />
Then I should see the field designation activity in submitted status <br />
And I should see the field designation in the planning phase of the growing season

#### Soil Sampling Scenarios

##### Scenario: Soil Sampling Done
Given I am working with one farmer <br />
And I have performed a soil sampling <br />
When I view the farmer's timeline <br />
Then I should see the soil sampling activity in done status <br />
And I should see the soil sampling in the planning phase of the growing season

### View Planting Growing Phase Activities

#### Story

As an agronomist <br />
I want to view all Planting activities sequentially <br />
So that I can ensure the farmer's fields produce the most yield for the harvest phase.

#### Planting (Activity) Scenarios

##### Scenario: Planting Done
Given I am working with one farmer <br />
And we have finished planting <br />
When I view the farmer's timeline <br />
Then I should see the planting activity in done status <br />
And I should see the planting in the planting phase of the growing season

#### Herbicide Scenarios

##### Scenario: Herbicide Planned
Given I am working with one farmer <br />
And I have planned herbicide treatment <br />
When I view the farmer's timeline <br />
Then I should see the herbicide activity in planned status <br />
And I should see the herbicide in the planting phase of the growing season

##### Scenario: Herbicide Done
Given I am working with one farmer <br />
And I have planned herbicide treatment <br />
And we have finished herbicide treatment <br />
When I view the farmer's timeline <br />
Then I should see the herbicide activity in done status <br />
And I should see the herbicide in the planting phase of the growing season

#### Insecticide Scenarios

##### Scenario: Insecticide Planned
Given I am working with one farmer <br />
And I have planned insecticide treatment <br />
When I view the farmer's timeline <br />
Then I should see the insecticide activity in planned status <br />
And I should see the insecticide in the planting phase of the growing season

##### Scenario: Insecticide Done
Given I am working with one farmer <br />
And I have planned insecticide treatment <br />
And we have finished insecticide treatment <br />
When I view the farmer's timeline <br />
Then I should see the insecticide activity in done status <br />
And I should see the insecticide in the planting phase of the growing season

#### Fertilizer Scenarios

##### Scenario: Fertilizer Planned
Given I am working with one farmer <br />
And I have planned fertilizer treatment <br />
When I view the farmer's timeline <br />
Then I should see the fertilizer activity in planned status <br />
And I should see the fertilizer in the planting phase of the growing season

##### Scenario: Fertilizer Done
Given I am working with one farmer <br />
And I have planned fertilizer treatment <br />
And we have finished fertilizer treatment <br />
When I view the farmer's timeline <br />
Then I should see the fertilizer activity in done status <br />
And I should see the fertilizer in the planting phase of the growing season

#### Observation Scenarios

##### Scenario: Observation Done
Given I am working with one farmer <br />
And I have done an observation <br />
When I view the farmer's timeline <br />
Then I should see the observation activity in done status <br />
And I should see the observation in the planting phase of the growing season

##### Scenario: Multiple Observations Done
Given I am working with one farmer <br />
And I have done an observation <br />
And I have done an observation <br />
And I have done an observation <br />
When I view the farmer's timeline <br />
Then I should see the three observation activities in done status <br />
And I should see the three observations in the planting phase of the growing season

#### Detasseling Scenarios

##### Scenario: Detasseling Planned
Given I am working with one farmer <br />
And I planned detasseling <br />
When I view the farmer's timeline <br />
Then I should see the detasseling activity in planned status <br />
And I should see the detasseling in the planting phase of the growing season

##### Scenario: Detasseling Done
Given I am working with one farmer <br />
And I planned detasseling <br />
When I view the farmer's timeline <br />
Then I should see the detasseling activity in done status <br />
And I should see the detasseling in the planting phase of the growing season

### View Harvest Growing Phase Activities

#### Story

As an agronomist <br />
I want to view all Harvest activities sequentially <br />
So that I can reap the rewards of Planning and Planting phase work.

#### Harvesting (Activity) Scenarios

##### Scenario: Harvesting Done
Given I am working with one farmer <br />
And we have finished harvesting <br />
When I view the farmer's timeline <br />
Then I should see the harvesting activity in done status <br />
And I should see the harvesting in the harvest phase of the growing season

#### Storage Scenarios

##### Scenario: Storage Done
Given I am working with one farmer <br />
And we have stored the crop <br />
When I view the farmer's timeline <br />
Then I should see the storage activity in done status <br />
And I should see the storarge in the harvest phase of the growing season

#### Delivery Scenarios

##### Scenario: Delivery Done
Given I am working with one farmer <br />
And we have delivered the crop to the co-op <br />
When I view the farmer's timeline <br />
Then I should see the delivery activity in done status <br />
And I should see the delivery in the harvest phase of the growing season

#### Sale Scenarios

##### Scenario: Sale
Given I am working with one farmer <br />
And we have sold the crop to the co-op <br />
When I view the farmer's timeline <br />
Then I should see the sale activity in sold status <br />
And I should see the sale in the harvest phase of the growing season

##### Scenario: Multiple Sales
Given I am working with one farmer <br />
And we have sold the crop to the co-op <br />
And we have sold the crop on the open market <br />
And we have sold the crop to another farmer <br />
When I view the farmer's timeline <br />
Then I should see three sale activities in sold status <br />
And I should see the sales in the harvest phase of the growing season