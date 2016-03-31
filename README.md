# unix-cheat-sheet

Make a file executable: `chmod a+x <filename>`

Switch to superuser: `suod su -` (the dash I think means current user)

Current time: `date`

List directory in order of modified: `ls -ltr`

Configure a cron job: `crontab -e` then `1 (minute) 0 (hour)  * * 3 (day of week) username <script path>`

Show processes on each port: `lsof`

List all processes: ` ps aux | grep cron`

Restart service: `service crond restart`

Repeat a command every n seconds: `watch -n n <command>`

#less

End of file: `shift+g`
Start of file: `shift+h`

```html
<!doctype html>
<html>

<head>
    <style>
    body {
    	color: #111;
        padding: 35px 150px;
        font-family: Helvetica;
        font-size: 16pt;
        line-height: 30pt;
        box-sizing: border-box;
    }
    
    h1 {
        display: inline;
    }
    
    table {
        width: 100%;
    }
    
    th {
        text-align: left;
        color: silver;
    }
    
    main {
        margin-top: 100px;
    }
    
    footer {
        margin-top: 100px;
        font-size: 1rem;
        color: silver;
    }
    
    #dates {
        float: right;
    }
    
    [data-type='annotated']::before {
        font-weight: bold;
        margin-right: 20px;
        color: silver;
        font-size: 1rem;
    }
    
    #date::before {
        content: 'Date';
    }

    #due::before {
        content: 'Due';
    }

    #invoicer::before {
        content: 'Invoicer';
    }
    
    #invoicee::before {
        content: 'Invoicee';
    }
    </style>
</head>

<body>
    <header>
        <header>
            <h1>Invoice</h1>
            <section id="dates">
                <div data-type='annotated' id="date">
                    dd/mm/yyyy
                </div>
                <div data-type='annotated' id="due">
                    dd/mm/yyyy
                </div>
            </section>
        </header>
        <main>
        	<section id="orgs">
                <div data-type='annotated' id="invoicee">
                    iKas Recruitment
                </div>
                <div data-type='annotated' id="invoicer">
                    Cloudsca.pe Software Development Limited
                </div>
            </section>
            <h2>Items</h2>
            <table>
                <tr>
                    <th>Date</th>
                    <th>Description</th>
                    <th>Units</th>
                    <th>Unit Cost</th>
                </tr>
                <tr>
                    <td>2016-03-01</td>
                    <td>Consultancy Services</td>
                    <td>1</td>
                    <td>1 GBP</td>
                </tr>
                <tr>
                    <td>2016-03-02</td>
                    <td>Consultancy Services</td>
                    <td>1</td>
                    <td>1 GBP</td>
                </tr>
                <tr>
                    <td>2016-03-03</td>
                    <td>Consultancy Services</td>
                    <td>1</td>
                    <td>1 GBP</td>
                </tr>
            </table>
        </main>
        <footer>
            <section id="company-name">
                Cloudsca.pe Software Development Limited.
            </section>
            <section id="registered-office">
                Registered office: Beech House Tydehams Newbury Berkshire, RG14 6JT.
            </section>
        </footer>
</body>

</html>
```
