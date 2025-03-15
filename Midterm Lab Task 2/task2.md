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
![Image](https://github.com/user-attachments/assets/592dfe22-bd3b-4126-8691-980c9cc1136c)

## Advanced Editor
![Image](https://github.com/user-attachments/assets/6e4720ad-a233-4bdb-8d33-1ee3827f8d00)
## States
![Image](https://github.com/user-attachments/assets/681e007c-1628-4394-969c-c14d7510dd87)
## Sal by Role Type
![Image](https://github.com/user-attachments/assets/a02e3c12-889c-4f93-9dd6-b10ec8276ddb)
## Sal by Role Size
![Image](https://github.com/user-attachments/assets/5ea71110-b656-48eb-ac68-98f2a55e7b72)
## Sal by State
![Image](https://github.com/user-attachments/assets/e4a0521e-0633-4f05-aa18-d29f755561b6)
## Query Dependencies
![Image](https://github.com/user-attachments/assets/1d639aca-e72d-46cd-944b-ceb6abc49cfd)
