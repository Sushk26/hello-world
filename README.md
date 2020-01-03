<exec when="init">
def PipeBrand():
    string = ""
    for x in S10.rows.order:
        if x.c4 and x.label != 'r97':
            string = string + "&lt;li&gt;" + x.text + "&lt;/li&gt;"
        if  x.c4 and x.label == 'r97':
            string = string + "&lt;li&gt;" + x.open + "&lt;/li&gt;"

    return string
 </exec>

    <html label="LastPurchaseIntro" where="survey"><b>${PipeBrand()}</b></html>
