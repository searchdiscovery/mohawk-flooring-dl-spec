![SDI Logo](https://www.searchdiscovery.com/wp-content/uploads/2017/03/SDI-Black.svg)

# DL - Flooring Sites (Pergo/Karastan/Mohawk)

## Overview
This repository contains the necessary specifications to build an event driven data layer.

## Adobe Launch Deployment
The following HTML should be deployed on your site(s), at the top of the "<head>" tag.
- Production: <script src="//assets.adobedtm.com/13496781d41f/b9bd22ab52ce/launch-f98e549ff183.min.js" async></script>
- Staging: <script src="//assets.adobedtm.com/13496781d41f/b9bd22ab52ce/launch-676fe9c5232d-staging.min.js" async></script>
- Dev:<script src="//assets.adobedtm.com/13496781d41f/b9bd22ab52ce/launch-96184724ee09-development.min.js" async></script>

## Data Layer
Each file inside the [events](/events/) folder corresponds to a single use case or site event that needs to be implemented.

These will be used to share data with the tag management tool of choice and to trigger the corresponding tracking events in the analytics tool of choice.

As the data layer is event-based, the order in which the events are fired is critical. In general, events will fire in teh following order:

Page Load Started > Other Page-level Events (Product Viewed, Product Listing Displayed, etc.) > Page Load Completed

Some events such as Product Interactions will be fired as they occur, where the above order is not needed as the view of a new page is not occuring.


## Questions/Comments
For any questions or comments, please contact jason.egan@searchdiscovery.com.
