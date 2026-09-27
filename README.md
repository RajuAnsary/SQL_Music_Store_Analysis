# Music Store Data Analysis

A SQL-based data analysis project using PostgreSQL to analyze an online music store database and answer business-oriented questions related to customers, invoices, artists, genres, and purchasing behavior.

---

##  Project Overview

This project analyzes a relational music store database using SQL to extract meaningful business insights.

The analysis focuses on:

- Customer purchasing behavior
- Invoice and revenue patterns
- Rock music listeners
- Top Rock artists
- Customer spending by artist
- Popular music genres by country
- Highest-spending customers by country
- Track duration analysis

The project demonstrates practical SQL skills including **JOINs, GROUP BY, aggregate functions, subqueries, CTEs, and window functions**.

---

## Technologies Used

- **PostgreSQL**
- **pgAdmin 4**
- **SQL**

---

## Database Schema

The database contains the following major tables:

- `album`
- `artist`
- `customer`
- `employee`
- `genre`
- `invoice`
- `invoice_line`
- `media_type`
- `playlist`
- `playlist_track`
- `track`

### Main Relationships

```text
Customer
   │
   ▼
Invoice
   │
   ▼
Invoice_Line
   │
   ▼
Track
   │
   ├──► Genre
   │
   └──► Album
          │
          ▼
        Artist
