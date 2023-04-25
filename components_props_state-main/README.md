QUESTION 1a: Google Page Component breakdown
Google App is the Parent component; within it we have three main components;
1. Header Component
2. Search Section Component
3. Footer Section
Within these components, we have subcomponents i.e

1. HEADER COMPONENT
i. Menu Item Components: Gmail and 
ii. Icon components -the Google Apps component icon
iii. Avatar component when logged in or Sign in component when not logged in.

2. SEARCH COMPONENT
i. Logo component i.e Google logo
ii. Search bar component
iii. Reporting component composed of the 
iv. Language component - lists of Google location based languages 

3. FOOTER SECTION
Section is composed of the top and bottom footer components, where
i. Top Footer is the country
ii. The Bottom Footer is a menu;
Left Menu comprised of About, Advertising,Business and How Search works links
Mid Menu the Carbon neutral link
Right Menu comprised of Privacy, Terms and Settings

QUESTION 2
To demostrate the use of State, the input section was modified as below;
export default function SearchBar() {
    const [value, setValue] = useState('');
    const onChange = (event) => {
        setValue(event.target.value);
    }
    return (
        <div ClassName="Bar">
            <input className="searchbar" type="Text" value={value} onChange={onChange} title="Search" />
            <a href="#"> <img className="search" src={Icon1} alt="search" /></a>
            <a href="#"> <img className="voice" src={Icon2} alt="voice search" /></a>
            <a href="#"> <img className="image" src={Icon3} alt="image search" /></a>

        </div>
    )
}


