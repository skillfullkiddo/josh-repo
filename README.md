# josh-repo
Joshua Address Book

<!DOCTYPE html>

<html>
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=0">
        <title>Page Title</title>
        <link rel="stylesheet" type="text/css" href="http://code.jquery.com/mobile/latest/jquery.mobile.min.css" />
        <script type="text/javascript" src="http://code.jquery.com/jquery-1.6.2.min.js"></script>
        <script type="text/javascript" src="http://code.jquery.com/mobile/latest/jquery.mobile.min.js"></script>

        <script type="text/javascript" src="store.js"></script>
        <script type="text/javascript" src="contacts.js"></script>
        <script type="text/javascript" src="add.js"></script>
        <script type="text/javascript" src="main.js"></script>
    </head>

    <body>
        <div data-role="page" id="page-main">
            <div data-role="header">
                <h1>Joshua's Address Book</h1>
                <a href="#page-add" id="add" data-icon="plus" class="ui-btn-right">Add</a>
            </div>

            <div data-role="content">
                <ul data-role="listview" id="all-contacts">
                </ul>
            </div>
        </div>

        <div data-role="page" id="page-add">
            <div data-role="header">
                <h1>Add Contact</h1>
            </div>

            <div data-role="content">
                <div data-role="fieldcontain">
                    <label for="name">Contact Name</label>
                    <input type="text" name="name" id="fld-name" value="" />
                </div>

                <div data-role="fieldcontain">
                    <label for="number">Phone Num</label>
                    <input type="tel" name="phone" id="fld-phone" value="" />
                </div>

                <div data-role="fieldcontain">
                    <label for="email">Email</label>
                    <input type="email" name="email" id="fld-email" />
                </div>

                <a href="#page-main" id="btn-save-contact" data-inline="true" data-role="button" data-theme="b" data-direction="reverse">Save</a>
                <a href="#page-main" data-inline="true" data-role="button" data-direction="reverse">Cancel</a>
            </div>

        </div>
        <div data-role="page" id="page-view">
            <div data-role="header">
                <h1>Contact Info</h1>
                <a href="#page-main" data-direction="reverse">Back</a>
            </div>

            <div data-role="content">
                <div><b>Name: </b><span id="view-name"></span></div>
                <div><b>Phone: </b><span id="view-phone"></span></div>
                <div><b>Email: </b><span id="view-email"></span></div>
            </div>
        </div>

    </body>

</html>
