
Follow the instruction to setup and access the contatc API.

********************************************************************
Setps to run the Contact API.
1. Copy the project at "Drive" C: (Or any present drive)
2. Build the project in Release mode using CPU type as Any CPU. you can also use the existing build binaries
3. The go the location '<Drive on which project was copied>\ContactAPI\Contact.Test\bin\Release\netcoreapp3.1\ContactServices.exe' and right click and Run as administartor.
4. Should able to see a black window appear and there is no error.

***************************************************************

****************************************************************

Instruction to use the API links

The Base Url of Contact API is "http://localhost:5000/api/v1.0" for HTTP and for HTTPS its "https://localhost:5001/api/v1.0

1. To get list of all contatc use: "<BaseUrl>/GetContactList"
2. Add new contact use : "<BaseUrl>/AddContact"
   The body request should be in format:
    {
	"firstName" : "TestFirstName",
	"lastName" : "TestLastName",
	"email" : "Test@Test.com",
	"phone" : "100000000000",
    "status" : "Active"
    }
3. Edit contact use: "<BaseUrl>/EditContact/{id} "
   In this id it the contat id, when add contact a guild is created for that contat.
4. Delete a contact use : "<BaseUrl>/DeleteContact/{id}"
5. Inactive a contact use : "<BaseUrl>/InactiveContact/{id}"
6. All the records are store in 'Contact.Json' file at location from where the application is running. For e.g <Drive at which project are copied and build>\ContactAPI\bin\Release\netcoreapp3.1\Contact.Json
7. You can see the records that are added in the above file 

*******************************************************************

