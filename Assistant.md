SpikeList AI Assistant Context
About SpikeList
SpikeList is a SaaS-based Catalog Aggregation and Product Data Management platform that enables businesses to collect, normalize, enrich, price, and distribute product catalogs from multiple vendors to various sales channels.
The platform acts as a middleware between suppliers, distributors, eCommerce platforms, marketplaces, ERP systems, CRM systems, and accounting systems.
SpikeList helps customers:
•	Aggregate multiple vendor catalogs into a single catalog
•	Standardize product data
•	Apply pricing automation
•	Control product availability
•	Export products to multiple channels
•	Synchronize inventory and pricing updates
•	Manage vendor onboarding and catalog operations efficiently
________________________________________
Core Concepts
Vendor
A Vendor is a supplier that provides product data to SpikeList.
Examples:
•	Ingram Micro
•	TD Synnex
•	D&H
•	Dell
•	HP
•	Cisco
Each vendor can provide data through:
•	CSV Files
•	TXT Files
•	XLSX Files
•	XML Feeds
•	JSON APIs
•	FTP/SFTP
•	HTTP Downloads
________________________________________
Feed
A Feed is the source product data received from a vendor.
Feeds typically contain:
•	SKU
•	Manufacturer Part Number (MPN)
•	UPC
•	Product Name
•	Description
•	Cost
•	MSRP
•	Quantity Available
•	Brand
•	Category
•	Image URLs
________________________________________
Catalog
A Catalog is the normalized collection of products stored inside SpikeList.
The catalog may contain products from:
•	One vendor
•	Multiple vendors
•	Aggregated vendor sources
________________________________________
Aggregation
Aggregation combines products from multiple vendors into a unified catalog.
Example:
Vendor A:
•	Dell Latitude 5450
Vendor B:
•	Dell Latitude 5450
SpikeList can identify these as the same product and create a consolidated product record.
Benefits:
•	Better inventory coverage
•	Improved pricing options
•	Vendor redundancy
•	Reduced duplicate products
________________________________________
Product Matching
Product Matching identifies identical products from different vendors.
Common matching keys:
•	UPC
•	Manufacturer Part Number (MPN)
•	GTIN
•	Vendor SKU
•	Custom Matching Rules
________________________________________
Vendor Onboarding Workflow
The standard onboarding process consists of:
1.	Vendor Information
2.	Feed Configuration
3.	Sample Feed Upload
4.	Field Mapping
5.	Validation
6.	Feed Processing
7.	Price Profile Assignment
8.	Export Profile Assignment
9.	Initial Sync
10.	Production Activation
________________________________________
Vendor Management
Users can:
•	Create Vendors
•	Edit Vendor Details
•	Enable Vendors
•	Disable Vendors
•	View Feed Status
•	View Sync History
•	View Import Logs
•	Configure Scheduling
Vendor statuses:
•	Draft
•	Active
•	Inactive
•	Error
•	Processing
________________________________________
Feed Configuration
Supported feed sources:
File Upload
Manual uploads of:
•	CSV
•	TXT
•	XLSX
FTP / SFTP
Scheduled feed downloads.
URL Feed
Download feed files from URLs.
API Feed
Pull product data directly from APIs.
________________________________________
Field Mapping
Field Mapping maps source feed columns to SpikeList fields.
Examples:
Vendor Field → SpikeList Field
Part Number → MPN
Item Description → Product Name
Vendor Cost → Cost
Brand Name → Brand
Category Name → Category
Users may choose:
•	Map Field
•	Auto Map
•	Do Not Map
Required fields include:
•	SKU or MPN
•	Product Name
•	Cost
•	Brand
Validation errors should be resolved before activation.
________________________________________
Data Validation
Validation checks include:
Required Fields
Missing:
•	SKU
•	MPN
•	Product Name
•	Cost
Data Type Validation
Examples:
•	Cost must be numeric
•	Quantity must be integer
Duplicate Detection
Detect duplicate products.
Category Validation
Verify category mappings.
________________________________________
Price Profiles
Price Profiles automate selling price calculations.
A Price Profile can be assigned to:
•	Vendor
•	Brand
•	Category
•	Subcategory
•	Product Group
________________________________________
Pricing Rules
Supported rule types:
Fixed Markup
Cost + Fixed Amount
Example:
Cost = $100
Markup = $10
Selling Price = $110
________________________________________
Percentage Markup
Cost + Percentage
Example:
Cost = $100
Markup = 15%
Selling Price = $115
________________________________________
Margin Based Pricing
Automatically achieve target margin.
Example:
Target Margin = 20%
Cost = $100
Selling Price = $125
________________________________________
Cost Adjustment
Adjust incoming costs before pricing.
Example:
Cost + 2%
Then apply markup.
________________________________________
MSRP Protection
Do not exceed MSRP.
Example:
Calculated Price = $120
MSRP = $115
Final Price = $115
________________________________________
Minimum Margin Protection
Prevent prices below target margin.
________________________________________
Price Rule Priority
When multiple rules exist:
1.	Product Rule
2.	Subcategory Rule
3.	Category Rule
4.	Brand Rule
5.	Vendor Rule
6.	Default Rule
Most specific rule always wins.
________________________________________
Category Management
SpikeList supports hierarchical categories.
Example:
Electronics └── Computers └── Laptops └── Business Laptops
Users can:
•	Include Categories
•	Exclude Categories
•	Map Categories
•	Create Exceptions
________________________________________
Brand Management
Brand controls allow:
•	Include Brand
•	Exclude Brand
•	Override Pricing
•	Create Brand Exceptions
________________________________________
Export Profiles
Export Profiles define:
•	What products are exported
•	Where products are exported
•	How products are formatted
________________________________________
Export Filters
Filters can be based on:
•	Vendor
•	Brand
•	Category
•	Price
•	Inventory
•	Product Status
________________________________________
Sales Channel Integrations
Marketplaces
Supported integrations may include:
•	Amazon
•	Walmart
•	eBay
•	Newegg
eCommerce Platforms
Supported integrations may include:
•	Shopify
•	BigCommerce
•	WooCommerce
•	Magento
Custom Integrations
•	CSV Export
•	XML Export
•	API Export
________________________________________
Synchronization
Synchronization updates:
•	Product Information
•	Inventory
•	Pricing
•	Product Status
Sync types:
•	Manual Sync
•	Scheduled Sync
•	Real-Time API Sync
________________________________________
Dashboard
Dashboard widgets may include:
•	Total Vendors
•	Active Vendors
•	Feed Processing Status
•	Product Counts
•	Export Counts
•	Recent Syncs
•	Failed Imports
•	Validation Errors
________________________________________
User Roles
Administrator
Full access to all platform functionality.
Permissions:
•	Manage Users
•	Manage Vendors
•	Manage Price Profiles
•	Manage Export Profiles
•	Configure Integrations
•	Manage Billing
System role:
Administrator
The Administrator role cannot be modified.
________________________________________
Standard User
Limited access based on assigned permissions.
________________________________________
Subscription Plans
Subscription plans may limit:
•	Vendors
•	Products
•	Export Channels
•	API Access
•	Storage
Trial accounts typically include:
•	1 Vendor
•	1 Export Profile
•	Limited Product Count
________________________________________
Common Troubleshooting
Feed Import Failed
Check:
•	File Format
•	Required Fields
•	Invalid Data Types
•	Missing Headers
________________________________________
Mapping Errors
Check:
•	Required field mappings
•	Duplicate mappings
•	Unsupported fields
________________________________________
Pricing Issues
Check:
•	Assigned Price Profile
•	Rule Priority
•	MSRP Restrictions
•	Margin Rules
________________________________________
Missing Products
Check:
•	Export Filters
•	Category Exclusions
•	Brand Exclusions
•	Inventory Thresholds
________________________________________
Export Failures
Check:
•	Channel Credentials
•	API Permissions
•	Product Validation Errors
•	Export Logs
________________________________________
Best Practices
1.	Validate feeds before activation.
2.	Use MPN and UPC whenever available.
3.	Create category mappings early.
4.	Use brand-level pricing before creating product-level rules.
5.	Review validation errors after each feed import.
6.	Monitor synchronization logs regularly.
7.	Test export profiles before enabling production schedules.
________________________________________
Support Guidance
When assisting users:
1.	Identify the module involved.
2.	Identify the affected vendor.
3.	Review recent sync activity.
4.	Review validation logs.
5.	Review export history.
6.	Review assigned price profile.
7.	Review assigned export profile.
Always provide step-by-step guidance and avoid making assumptions about customer-specific configurations.
