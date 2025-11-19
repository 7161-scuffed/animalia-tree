# Animalia Tree Project

A buffer-loaded, editable evolutionary tree with Google Slides-style genus entry and editing.

## Structure
- `/backend`: Express/MongoDB API, buffered genus loading, slide data model
- `/frontend`: React app, virtualization, drag & drop genus slide editor, slideshow per genus

## Getting Started
1. Start MongoDB locally (port 27017)
2. `cd backend && npm install` (install express, mongoose, body-parser, cors)
3. `node server.js`
4. `cd ../frontend && npm install`
5. `npm start`

## Bulk Data Loader
- Place genus_data.json (from GBIF, Catalogue of Life, etc.) in `/backend/scripts/`
- Run: `node scripts/loadGenusData.js`

## Frontend Features
- Buffered virtual tree, never freezes — expands on demand
- Genus "slide deck" for anatomical drawings, maps, images
- Full Google Slides-style editing of slides
- Fact-checked fields and extensible genus info

## Advanced
- Extend genus schema, slide layouts, or add new slide data types as needed
