# Digitalization-of-the-Hospitality-Process-Project

## Objective
Develop a web application to facilitate digitalizing the hospitality process for group accommodation. The application allows users to upload two CSV files to efficiently allocate rooms in hostels, ensuring group members with the same ID stay together while adhering to hostel capacities and gender-specific accommodations.

## Features
- **Upload CSV Files:** Users can upload two CSV files—one containing group information and another containing hostel information.
- **Room Allocation Algorithm:** An algorithm allocates rooms based on group IDs, gender-specific hostels, and room capacities.
- **Display Allocations:** The application displays the allocated rooms, indicating which group members are in which room.
- **Downloadable CSV:** Users can download a CSV file with the room allocation details.

## Project Structure
```
project
├── node_modules
├── project-directory
│   ├── public
│   ├── routes
│   │   └── upload.js
│   ├── views
│   │   └── index.ejs
├── app.js
├── package-lock.json
├── package.json
```

## Logic
1. **CSV File Upload:** Users upload two CSV files—one for group information and one for hostel information.
2. **Parsing CSV Files:** The application parses the CSV files to extract group and hostel information.
3. **Room Allocation Algorithm:**
   - Groups are allocated rooms based on their size and gender.
   - Members of the same group are placed in the same room as much as possible.
   - Boys and girls are placed in their respective hostels.
   - Room capacity is not exceeded.
4. **Display Allocations:** The application displays the allocation results on the frontend.
5. **Download CSV:** Users can download the allocation details as a CSV file.

## Instructions to Run the Application

1. **Clone the Repository:**
   Open your terminal or command prompt and run the following command to clone the repository:
   ```bash
   git clone https://github.com/bytebender77/Web_Digitalization-of-the-Hospitality-Process-Project.git
   cd Web_Digitalization-of-the-Hospitality-Process-Project
   ```

2. **Open in Visual Studio Code:**
   Open Visual Studio Code and navigate to the cloned repository directory.

3. **Install Dependencies:**
   Make sure you have Node.js installed. Then, open the terminal in VS Code and run:
   ```bash
   npm install
   ```

4. **Run the Application:**
   In the VS Code terminal, start the application by running:
   ```bash
   node app.js
   ```

5. **Access the Application:**
   Open your web browser and navigate to `http://localhost:3000` to access the application.

## Usage
1. **Upload CSV Files:** On the homepage, upload the `Group Information` CSV file and the `Hostel Information` CSV file.
2. **View Allocations:** Click on the button to allocate rooms. The allocations will be displayed on the screen.
3. **Download CSV:** Click the download button to save the allocation details as a CSV file.

## Example
- **Group Information CSV:**
  ```csv
  Group ID,Members,Gender
  101,3,Boys
  102,4,Girls
  103,2,Boys
  104,5,Girls
  105,8,5 Boys & 3 Girls
  ```
- **Hostel Information CSV:**
  ```csv
  Hostel Name,Room Number,Capacity,Gender
  Boys Hostel A,101,3,Boys
  Boys Hostel A,102,4,Boys
  Girls Hostel B,201,2,Girls
  Girls Hostel B,202,5,Girls
  ```

## Repository Link
[Web Digitalization of the Hospitality Process Project](https://github.com/bytebender77/Web_Digitalization-of-the-Hospitality-Process-Project.git)

---

Submit this GitHub repository link in the provided Google form. Ensure your code is well-commented and organized for clarity. If you need any further assistance, feel free to ask!
