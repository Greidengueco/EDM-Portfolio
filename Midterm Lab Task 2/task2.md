# Midterm Lab Task 2 – Data Cleaning with Power Query**  

This portfolio shows how to clean and prepare data using Power Query. The dataset has multiple tables that need cleaning to improve quality and consistency before analysis.  

### Steps:  

1. **Load Data**  
   - Download *Uncleaned_DS_jobs.csv*  
   - Open in Excel → Data → New Query → Open File → Text/CSV → Load & Edit in Power Query  

2. **Duplicate Raw Data**  
   - Right-click dataset → Select Duplicate  

3. **Clean Salary Data**  
   - Select *Salary Estimate* → Extract text before "("  
   - Create *Min Salary* and *Max Salary* columns using *Column from Examples*  

4. **Add Role Type**  
   - Create a *Custom Column* → Assign roles based on job titles (*Data Scientist, Data Analyst, etc.*)  

5. **Split Location Column**  
   - Add *State Abbreviation* column with corrections (e.g., *New Jersey → NJ*)  
   - Split *Location* by comma → Rename second column as *State Abbreviations*  

6. **Split Company Size**  
   - Create *MinCompanySize* and *MaxCompanySize* using Salary Estimate method  

7. **Handle Negative Values**  
   - Remove *-1s* and *0s* from *Competitors, Revenues, and Industry*  

8. **Clean Company Names**  
   - Remove extra characters or ratings after company names  

9. **Save Cleaning Steps**  
   - Copy Power Query code from *Advanced Editor* and save  

10. **Reshape & Group Data**  
   - Group by *Role Type* → Get avg. Min/Max Salary (convert to currency, multiply by 1000)  
   - Group by *Company Size* → Get avg. Min/Max Salary  

11. **Merge State Mapping**  
   - Merge *State Abbreviation* with *State Mapping* query  
   - Rename merged column as *State Full Name* → Remove nulls  

12. **Group by State**  
   - Group by *State Full Name* → Get avg. Min/Max Salary  

13. **Check Query Links**  
   - Go to *View → Dependencies* → Ensure correct links

# Screenshots
## Cleaned Table
![Image](https://github.com/user-attachments/assets/77422a33-4267-4cfc-b933-1bcc93882ac2)

## Advanced Editor
![Image](https://github.com/user-attachments/assets/6e4720ad-a233-4bdb-8d33-1ee3827f8d00)
## States
![Image](https://github.com/user-attachments/assets/f2f54708-338a-4a73-8c87-56b1c5a731ed)
## Sal by Role Type
![Image](https://github.com/user-attachments/assets/7b3dbc37-9950-41b5-a3b1-8a2955ff33ec)
## Sal by Role Size
![Image](https://github.com/user-attachments/assets/c62e617e-12a0-4566-b883-19d0ffd1ca64)
## Sal by State
![Image](https://github.com/user-attachments/assets/e174b0b2-0e46-4d77-ad84-56ac946c5a95)
## Query Dependencies
![Image](https://github.com/user-attachments/assets/1d639aca-e72d-46cd-944b-ceb6abc49cfd)
