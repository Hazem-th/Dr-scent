# Dr-scent
<html>
<head>
    <meta charset="utf-8" />
    <meta http-equiv="Content-Type" content="text/html;charset=ISO-8859-1" />
    <meta name="viewport" content="width=device-width,initial-scale=1.0,user-scalable=no" />
    <meta name="google" content="notranslate" />
    <title>DR. SCENT</title>
    <script type="text/javascript" charset="utf-8" src="https://code.jquery.com/jquery-3.6.4.min.js" integrity="sha256-oP6HI9z1XaZNBrJURtCoUT5SUnxFr8s3BzRl+cbzUq8=" crossorigin="anonymous"></script>
<style>
    .ap-FormContainer{width:100%;margin:0 0;padding:1px;font-size:0.9rem !important}
    .ap-FormContainer form{margin:16px auto;max-width:600px}
    .ap-FormContainer h2{display:block;margin:2px 0 8px 0;padding:16px;text-align:center;}
    .ap-FormContainer form p{display:block;margin:12px!important;overflow:hidden}
    .ap-FormContainer form p label{display:block;border:none;margin:0 0;}
    .ap-FormContainer form p input[type=text]{padding:4px;display:block;border:1px solid #ccc;width:100%;height:2rem;}
    .ap-FormContainer form p span{display:inline-block;width:32%;padding:6px 2px;overflow:hidden;height:1.2rem!important;white-space:nowrap;}
    .ap-FormContainer form p span input[type=radio]{display:inline-block;}
    .ap-FormContainer form p span label{display:inline-block;}
    .ap-FormContainer form div{padding:12px 4px;overflow:hidden;display:block;width:100%;text-align:right;}
    .ap-FormContainer form div button{margin:8px;border:none;display:inline-block;padding:8px 32px;vertical-align:middle;overflow:hidden;text-decoration:none;
        box-shadow:0 2px 4px 0 rgba(0,0,0,0.2),0 1px 5px 0 rgba(0,0,0,0.19);text-align:center;cursor:pointer;white-space:nowrap;}
    .ap-FormContainer form div button:disabled{cursor:not-allowed;opacity:0.3;pointer-events:none}
    .ap-FormContainer form div button:hover{color:#000!important;background-color:#ccc!important;box-shadow:none;}
    @media(max-width:639px){.ap-FormContainer form p span{width:42%;}}
    @media(max-width:479px){.ap-FormContainer form p span{width:100%;}}
</style>
</head>
<body lang="en" style="background-color: #eae8e8;">
    
    <div class="ap-FormContainer"  >
        <img style="width: 200px !important; height: auto; margin:auto !important;" src="Artboard_6_1_1_.png" alt="Dr-scent !">
        <form id="LeadsAddFrm" autocomplete="off" autocorrect="off" spellcheck="false" style="border: 2px solid #ccc;border-radius: 8px;background-color: #f8f8f8;" >
            
            <h2>New platinum subscription</h2>
            <p id="LeTypeIDp">
                <label>Type</label>
                <span><input type="radio" name="LeTypeID" id="LeTypeID1" value="1" checked><label for="LeTypeID1">Private Co.</label></span>
                <span><input type="radio" name="LeTypeID" id="LeTypeID2" value="2"><label         for="LeTypeID2">Governmental Co.</label></span>
                <span><input type="radio" name="LeTypeID" id="LeTypeID0" value="0"><label         for="LeTypeID0">Personal</label></span>
            </p>
            <p id="LeNamep">
                <label>Name</label>
                <input id="LeName" name="LeName" type="text" autocomplete="off" autocorrect="off" spellcheck="false" minlength="0" maxlength="96" onkeyup="ValidateTextFunc(this)" onpaste="ValidateAndTrimFunc(this)" onfocusout="ValidateAndTrimFunc(this)" onchange="ValidateAndTrimFunc(this)" required>
            </p>
            <p id="LeEmailp">
                <label>Email</label>
                <input id="LeEmail" name="LeEmail" type="text" onkeyup="ValidateTextFunc(this)" onpaste="ValidateAndTrimFunc(this)" onfocusout="ValidateAndTrimFunc(this)" onchange="ValidateAndTrimFunc(this)" minlength="6" maxlength="32" pattern="[a-z0-9._%+-]+@[a-z0-9.-]+.[a-z]{2,3}$" title="The format should be suitable for e-mail , Attention must be lowercase letter,Example: aaaaaaaa@bbbb.com" required>
            </p>
            <p id="LePhonep">
                <label>Mobile Number</label>
                <input id="LePhone" name="LePhone" type="text" value="971" onkeyup="ValidateTextFunc(this)" onpaste="ValidateAndTrimFunc(this)" onfocusout="ValidateAndTrimFunc(this)" onchange="ValidateAndTrimFunc(this)" minlength="6" maxlength="16" pattern="[0-9]{6,16}$" title="Between 4 and 16 digits without spaces or letters" required>
            </p>
            <p id="LeZoneIDp">
                <label>Region</label>
                <span><input type="radio" name="LeZoneID" id="LeZoneID1"  value="1" checked><label for="LeZoneID1">Dubai</label></span>
                <span><input type="radio" name="LeZoneID" id="LeZoneID2"  value="2" ><label for="LeZoneID2">Abu Dhabi</label></span>
                <span><input type="radio" name="LeZoneID" id="LeZoneID3"  value="3" ><label for="LeZoneID3">AL Shariqah</label></span>
                <span><input type="radio" name="LeZoneID" id="LeZoneID4"  value="4" ><label for="LeZoneID4">Al Fujayrah</label></span>
                <span><input type="radio" name="LeZoneID" id="LeZoneID5"  value="5" ><label for="LeZoneID5">Umm al Qaywayn</label></span>
                <span><input type="radio" name="LeZoneID" id="LeZoneID6"  value="6" ><label for="LeZoneID6">Ras al Khaymah</label></span>
                <span><input type="radio" name="LeZoneID" id="LeZoneID7"  value="7" ><label for="LeZoneID7">Ajman</label></span>
                <span><input type="radio" name="LeZoneID" id="LeZoneID8"  value="8" ><label for="LeZoneID8">Al Ain</label></span>
                <span><input type="radio" name="LeZoneID" id="LeZoneID99" value="99"><label for="LeZoneID99">Other</label></span>            
            </p>
            <p id="LeAddressp">
                <label>Address</label>
                <input id="LeAddress" name="LeAddress" type="text" autocomplete="off" autocorrect="off" spellcheck="false" maxlength="64" onkeyup="ValidateTextFunc(this)" onpaste="ValidateAndTrimFunc(this)" onfocusout="ValidateAndTrimFunc(this)" onchange="ValidateAndTrimFunc(this)">
            </p>
            <p id="LeLeaderp">
                <label>How Did You Hear About DR. SCENT</label>
                <span><input type="radio" name="LeLeader" id="LeLeader0" value="Instagram" checked><label for="LeLeader0">Instagram</label></span>
                <span><input type="radio" name="LeLeader" id="LeLeader1" value="Facebook"><label for="LeLeader1">Facebook</label></span>
                <span><input type="radio" name="LeLeader" id="LeLeader2" value="Twitter"><label for="LeLeader2">Twitter</label></span>
                <span><input type="radio" name="LeLeader" id="LeLeader3" value="YouTube"><label for="LeLeader3">YouTube</label></span>
                <span><input type="radio" name="LeLeader" id="LeLeader4" value="TikTok"><label for="LeLeader4">TikTok</label></span>
                <span><input type="radio" name="LeLeader" id="LeLeader5" value="Search Engine"><label for="LeLeader5">Search engine</label></span>
                <span><input type="radio" name="LeLeader" id="LeLeader6" value="Friend"><label for="LeLeader6">Friend</label></span>
                <span><input type="radio" name="LeLeader" id="LeLeader7" value="Sales Representative"><label for="LeLeader7">Sales representative</label></span>
                <span><input type="radio" name="LeLeader" id="LeLeader8" value="Other"><label for="LeLeader8">Other</label></span>
            </p>
            <p id="LeDisCodep">
                <label>Discount Code</label>
                <input id="LeDisCode" name="LeDisCode" type="text" autocomplete="off" autocorrect="off" spellcheck="false" maxlength="64" onkeyup="ValidateTextFunc(this)" onpaste="ValidateAndTrimFunc(this)" onfocusout="ValidateAndTrimFunc(this)" onchange="ValidateAndTrimFunc(this)">
            </p>
            <div>
                <button id="LeadsBtn" type="submit">OK</button>
            </div>
        </form>
    </div>
</body>
<script type="text/javascript" charset="utf-8">
    $("#LeadsAddFrm").submit(function(event){
        $("#LeadsBtn").attr("disabled",true);
        var data=$(this).serialize();
        $.post("https://api.dr-scent.org/LeadsCreat.asp?C=DS2023_en",data).done(function(result){
            if(result[0].Res==0){$("#LeadsBtn").removeAttr("disabled")};
        }).done(function(){
            $("#LeadsAddFrm").html("Done");
        }).fail(function(){
            $("#LeadsAddFrm").html("Error");
        });
        return false
    });
//----------
function ValidateAndTrimFunc(e){
    var A=$.trim(e.value),B='',C='';
    for(let n=0;n<A.length;n++){
        B=A.substring(n,n+1);
        if(B.charCodeAt(0)==9||B.charCodeAt(0)==13){C+=" "}else
        if(B!="'"&&B!='"'&&B!='~'&&B!='|'&&B!=";"&&B!="%"&&B!="\\"&&B!="/"){C+=B};
    };
    if(e.id=='LePhone'){
        if(C.length>3){if(C.substring(0,3)!='971'){C='971'+C}};
    }else if(e.id=='LeEmail'){
        C=C.toLowerCase();
    };
    e.value=C;
}
//----------
function ValidateTextFunc(e){
    var A=e.value,B='',C='';
    for(let n=0;n<A.length;n++){
        B=A.substring(n,n+1);
        if(B.charCodeAt(0)==9||B.charCodeAt(0)==13){C+=" "}else
        if(B!="'"&&B!='"'&&B!='~'&&B!='|'&&B!=";"&&B!="%"&&B!="\\"&&B!="/"){C+=B};
    };
    if(e.id=='LePhone'){
        if(C.length>3){if(C.substring(0,3)!='971'){C='971'+C}};
    }else if(e.id=='LeEmail'){
        C=C.toLowerCase();
    };
    e.value=C;
}
//----------
</script>
</html>
