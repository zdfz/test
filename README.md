# District Clustering Tool

A web-based tool for visualizing and clustering districts based on geographical data and order quantities. This tool helps in optimizing delivery zones by grouping districts into balanced clusters.

## Features

- Interactive map visualization using Leaflet.js
- Dynamic district clustering with adjustable number of clusters
- Real-time cluster generation and visualization
- Detailed cluster statistics and summaries
- Support for GeoJSON data from Excel files
- Responsive design for both desktop and mobile devices

## Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Excel file with district data in the following format:
  - District name
  - GeoJSON coordinates
  - Order quantities
  - City information

## Usage

1. Prepare your Excel file (`districts_GeoJSON.xlsx`) with the required data
2. Open `district_clusters.html` in your web browser
3. Use the slider to adjust the number of desired clusters
4. Click "Generate Clusters" to create the district clusters
5. View the results on the map and in the sidebar summary

## Data Format

The Excel file should contain the following columns:
- District name
- GeoJSON (Polygon or MultiPolygon format)
- Order quantity
- City name

## Technical Details

- Built with vanilla JavaScript
- Uses Leaflet.js for map visualization
- Implements a custom clustering algorithm that balances:
  - Spatial proximity
  - Order quantity distribution
  - Geographical constraints

## Clustering Algorithm

The tool uses an optimized clustering algorithm that:
1. Initializes clusters using a K-means++ style approach
2. Assigns districts to clusters based on spatial proximity and order quantity
3. Performs iterative refinement to improve cluster balance
4. Maintains geographical contiguity where possible

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Support

For support, please open an issue in the repository. 
