# Sharepoint
project
To create a SharePoint hosted APP with Visual Studio 2017
Step1: 
Open the visual studio and to create new project, select office share left menu and choose the SharePoint add in from right side and give name as HelloWorldApp. And press Ok. Your project is created
 
Step2:
Default.aspx:  After creating the project from solution explorer  you select the Dfault .aspx file and delete the unnessary things for nice watching.

 
Code:

<%@ Page Inherits="Microsoft.SharePoint.WebPartPages.WebPartPage, Microsoft.SharePoint, Version=15.0.0.0, Culture=neutral, PublicKeyToken=71e9bce111e9429c" MasterPageFile="~masterurl/default.master" Language="C#" %>

<%@ Register TagPrefix="Utilities" Namespace="Microsoft.SharePoint.Utilities" Assembly="Microsoft.SharePoint, Version=15.0.0.0, Culture=neutral, PublicKeyToken=71e9bce111e9429c" %>
<%@ Register TagPrefix="WebPartPages" Namespace="Microsoft.SharePoint.WebPartPages" Assembly="Microsoft.SharePoint, Version=15.0.0.0, Culture=neutral, PublicKeyToken=71e9bce111e9429c" %>
<%@ Register TagPrefix="SharePoint" Namespace="Microsoft.SharePoint.WebControls" Assembly="Microsoft.SharePoint, Version=15.0.0.0, Culture=neutral, PublicKeyToken=71e9bce111e9429c" %>


<asp:Content ContentPlaceHolderID="PlaceHolderMain" runat="server">

    <div>
       <h1>Hello World</h1>
        <img src="../Images/images.jpg" />
    </div>

</asp:Content>

Step3:
ClienthostApp:
From solution explorer select HelloWorldApp and right click –select Add –new item –select Client web part(Host web), then give the HelloWorldApp and press ok .
 


Step4:
After creating client host app .delete the unnesseary things for nice watching. And Html body tag I wrote only hello world and drag image ( domensions:96*96).
 
Code:
<%@ Page language="C#" Inherits="Microsoft.SharePoint.WebPartPages.WebPartPage, Microsoft.SharePoint, Version=15.0.0.0, Culture=neutral, PublicKeyToken=71e9bce111e9429c" %>
<%@ Register Tagprefix="SharePoint" Namespace="Microsoft.SharePoint.WebControls" Assembly="Microsoft.SharePoint, Version=15.0.0.0, Culture=neutral, PublicKeyToken=71e9bce111e9429c" %>
<%@ Register Tagprefix="Utilities" Namespace="Microsoft.SharePoint.Utilities" Assembly="Microsoft.SharePoint, Version=15.0.0.0, Culture=neutral, PublicKeyToken=71e9bce111e9429c" %>
<%@ Register Tagprefix="WebPartPages" Namespace="Microsoft.SharePoint.WebPartPages" Assembly="Microsoft.SharePoint, Version=15.0.0.0, Culture=neutral, PublicKeyToken=71e9bce111e9429c" %>

<WebPartPages:AllowFraming ID="AllowFraming" runat="server" />

<html>
<head>
    <title></title>

    
</head>
<body>
    <h1>Hello world App</h1>
    <img src="../Images/images.jpg" />
</body>
</html>


Then run it. After few mins you got result default site. Then you can select developer site . –Page  -edit-insert-App Part- select your app Hellow world title then add it.
 
Now you will see your app in dev site.
 






Create App:
To cretae app for use another  people or company rightclick HelloWorldApp –publish- clickpackage the add in and save it.
 

 

