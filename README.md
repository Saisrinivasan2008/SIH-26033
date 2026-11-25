# Smart India Hackathon Workshop
# Date: 25/11/2026
## Reference Number: 26018086
## Name: T.S.Sai Srinivasan

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
KisanConnect is a digital marketplace where farmers and Farmer Producer Organizations (FPOs) list their produce and sell directly to consumers and bulk buyers such as restaurants, retailers, hostels, and processors. Farmers list the crop, quantity, quality grade, and expected price through a simple mobile app in regional languages like Tamil and Hindi, with voice input for users who are not comfortable typing. Buyers browse listings, place retail or bulk orders, and pay securely through UPI. The platform also matches each order with nearby transport providers and cold storage, and an AI engine forecasts demand so farmers know what to sell, when to sell, and at what fair price.

The platform addresses the problem by removing the layers of middlemen between farmers and buyers, so farmers keep a larger share of the final price while consumers pay less. Price transparency stops farmers from being underpaid, shorter supply chains reduce spoilage, and pooled shipments with optimized routes bring transport costs down.

What makes the solution unique is the combination of AI demand forecasting, shared-load route optimization where several farmers' produce travels on one truck, and a voice-first multilingual interface built for rural users. It also offers a fair-price indicator based on mandi rates and demand trends, along with farm-to-buyer traceability through a QR code on each batch.

## Technical Approach
The web frontend can be built with React.js and Tailwind CSS, and the mobile app with React Native or Flutter. The backend can run on Node.js with Express or Python with FastAPI, using PostgreSQL for users and orders and MongoDB for produce listings. The AI layer uses Python with scikit-learn and Prophet or LSTM models for demand forecasting, and Google OR-Tools for route optimization. Maps can come from Google Maps or OpenStreetMap, payments through Razorpay or a UPI gateway, and regional language and speech support through the Bhashini API. Everything can be containerized with Docker and hosted on AWS or Azure, with data pulled from Agmarknet, e-NAM, and a weather API.

The process begins with farmers, FPOs, and buyers registering with OTP verification. Farmers then upload produce details and photos, and the system suggests a fair price. Buyers search for produce or post their demand, and the system matches them by location, quantity, and quality. Once an order is placed, the buyer pays through UPI and the amount is held in escrow. The route optimizer assigns a vehicle, groups nearby pickups, and generates the most efficient route. After delivery, the buyer confirms receipt and the payment is released to the farmer. All sales data then feeds back into the forecasting model to improve future predictions.

For the flow chart, the sequence is: farmer lists produce, AI suggests a price, buyer places an order, payment is held in escrow, route optimization assigns transport, delivery happens, the buyer confirms, and payment is released. I'd recommend drawing this in draw.io or Figma and adding screenshots of a basic working prototype, such as the listing page and order page.

## Feasibility and Viability
The idea is technically feasible because every tool involved is open source or widely available, which makes a working prototype realistic within a hackathon timeline. Economically, the platform can earn through a small commission of one to three percent per order, logistics fees, and premium analytics for FPOs. Operationally, existing FPOs, Krishi Vigyan Kendras, and village-level agents can help with onboarding, and the idea aligns well with Digital India, e-NAM, and the government's FPO promotion scheme.

The main challenges are low digital literacy and poor internet connectivity in rural areas, farmers' initial distrust of online selling and payments, variation in produce quality, high last-mile delivery costs, and the cold-start problem of having too few buyers or sellers at launch. Perishable goods and volatile prices add further risk.

These can be overcome with a voice-first, regional-language app that has an offline mode and SMS or WhatsApp ordering, along with trained village-level "Kisan Mitra" agents who help farmers get started. Launching as a pilot in one district before scaling lets the team build trust gradually. Photo verification and buyer ratings maintain quality, partnerships with local transporters and cold storage keep logistics affordable, and escrow payments protect both sides.

## Impact and Benefits
Farmers and FPOs benefit from higher income through direct market access and fair pricing, while consumers get fresher produce at lower prices. Bulk buyers gain a reliable supply with transparent sourcing, and the wider rural economy gains new jobs in local logistics and agent networks.

Socially, the platform empowers small farmers financially and makes the rural economy more inclusive. Economically, fewer intermediaries mean a bigger share for farmers and lower prices for consumers. Environmentally, it reduces food waste, avoids empty truck trips, and lowers fuel use through optimized routes.

## Research and References
You can cite the e-NAM portal at enam.gov.in, Agmarknet at agmarknet.gov.in for mandi price data, the Open Network for Digital Commerce at ondc.org, and Bhashini at bhashini.gov.in for Indian language AI. The Ministry of Agriculture and Farmers Welfare's FPO scheme documents, the SIH 26033 problem statement from the Ministry of Consumer Affairs, Food and Public Distribution, and NITI Aayog or RBI reports on agricultural price spread and the farmer's share of consumer prices are also relevant. 

