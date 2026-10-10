# SchoolDirectoryApp# School Directory Dashboard

## Project Description
A Blazor web application that retrieves school information from the Edutots School API and presents it in a searchable directory with a details panel. Users can search by name, address or phone number, sort the list, mark favourites and view full details for each school.

## Technologies Used
- .NET 8
- Blazor Web App (Interactive Server)
- C#
- HttpClient with System.Text.Json
- LINQ
- CSS (custom styling, responsive layout)

## API Endpoint
https://edutots.net/api/school

The API also returns sensitive fields such as passwords. The app deliberately does not map or display them; only the seven required fields are used.

## Features
- Fetches and deserializes API data into a C# model
- Live, case-insensitive search by name, address or phone number
- School details panel
- Loading state and error handling with a retry option
- Reusable components using [Parameter] and EventCallback
- Sorting, favourites, refresh button and statistics (optional features)

## Project Structure
- Models/School.cs
- Services/ISchoolService.cs and SchoolService.cs
- Components/SchoolCard.razor and SchoolDetails.razor
- Components/Pages/Schools.razor

## How to Run
1. Install the .NET 8 SDK
2. Clone the repository: `git clone <your-repo-url>`
3. Open the folder: `cd SchoolDirectoryApp`
4. Run: `dotnet run`
5. Open the URL shown in the terminal and go to `/schools`
