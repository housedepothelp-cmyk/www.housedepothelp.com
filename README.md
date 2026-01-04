# backend/clearance_engine.py
import requests

def fetch_clearance_items():
    # Pull NJ Home Depot clearance items here
    # Filter 10%-100% off
    return [{"name":"Drill", "price":49.99, "store":"NJ Store"}]

def fetch_penny_items():
    # Pull items priced at $0.01
    return [{"name":"Screwdriver", "price":0.01, "store":"NJ Store"}]

def update_database():
    clearance = fetch_clearance_items()
    penny = fetch_penny_items()
    # Save to DB (placeholder)
    print("DB updated:", len(clearance), "clearance items,", len(penny), "penny items")
