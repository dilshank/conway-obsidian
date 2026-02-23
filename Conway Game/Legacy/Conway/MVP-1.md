# MVP 1


### Population dynamics on Map Sri Lanka
- population by GN (male/female)
- admin boundaries for DS
- traffic levels if available

### Core Simulations

Common:
- Users (identities that can theoretically be in more than one World)
- Worlds (these contain distinct universes in the game. Every asset and transaction is tied to a World ID)

In-World
- Entities (User IDs, Business IDs, Government ID)
- Business (stores distinct businesses)
	- Share Transactions (+ a View of current ownership)
	- Can be public or private
	- Businesses have types (some types are special - insurance, bank)
	- Government is a business**
- Stock Market (lists listed Businesses + meta data about them)
	- transaction ledger (as prices move) + view on current snapshot
- Land Registry (lists all available land in the World)
	- Land Transaction (+ a View of current ownership)
	- Owner can be Entity ID (User ID or Business ID)
- Asset Registry (lists all available assets to an Entity ID. Initially tracking Buildings.)
	- Each asset type has a dedicated reference table and registry
- Commodities Market
	- transaction ledger (as prices move) + view on current snapshot
- Impex Market (the great beyond your country listed as a common Impex Market)
	- transaction ledger (as prices move) + view on current snapshot
- Things Ledger
	- ownership of Things tracked (including where they're currently stored)
	- transaction ledger (as ownership changes) + view on current snapshot
	- Things can be created AND destroyed/consumed
	- units matter (1 tonne of tea, 1000 barrels of crude oil etc.)
- Bank Ledger
	- by Entity
	- transaction ledger (as ownership changes) + view on current snapshot
	- even things like btc are tracked with a special "crypto" bank
- Insurance Ledger**
	- policies owned by Entity