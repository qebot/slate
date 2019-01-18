# Businesses

Businesses are core to managing your franchises inside of Qebot.
The Business object stores data not only about business information, but also information that dictates how purchases are made.


## Business Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
business_name | <i class="item-label">string</i><br>| Name of the business.
category | <i class="item-label">Category</i> | See [Category](#category-object) object
phone  | <i class="item-label">string</i>| A phone contact number of the busieness.
fax  | <i class="item-label">string</i> | A fax number for the busieness.
address  | <i class="item-label">string</i>| Address of the business.
address2  | <i class="item-label">string</i> | Extra information for business address.
city  | <i class="item-label">string</i>| City of the business.
state_id  | <i class="item-label">State</i> | See [State](#state-object) object
state  | <i class="item-label">string</i> | Name of the state where address resides.
country  | <i class="item-label">Country</i>| See [Country](#country-object) object
zipcode  | <i class="item-label">string</i>| Zipcode of the business.
email  | <i class="item-label">string</i>| Contact email for the business.
website  | <i class="item-label">string</i>| Website for the business.
status  | <i class="item-label">string</i>| Status of the business.<br />Possible values: (<b>active</b>, <b>inactive</b>)

## Category Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
name | <i class="item-label">string</i><br>| Name of the category.
description | <i class="item-label">string</i> | Description of category.

### Possible Categories

<code>
  Categories<br />
&nbsp; <var><b>id</b> 1<br /><b>name</b> Accounting<br /><b>description</b> Accounting</var><br /><br />
&nbsp; <var><b>id</b> 2<br /><b>name</b> Advertising<br /><b>description</b> Advertising </var><br /><br />
&nbsp; <var><b>id</b> 3<br /><b>name</b> Aerospace<br /><b>description</b> Aerospace</var><br /><br />
&nbsp; <var><b>id</b> 4<br /><b>name</b> Agriculture<br /><b>description</b> Agriculture</var><br /><br />
&nbsp; <var><b>id</b> 5<br /><b>name</b> Aircraft<br /><b>description</b> Aircraft</var><br /><br />
&nbsp; <var><b>id</b> 6<br /><b>name</b> Airline<br /><b>description</b> Airline</var><br /><br />
&nbsp; <var><b>id</b> 7<br /><b>name</b> Apparel<br /><b>description</b> Apparel</var><br /><br />
&nbsp; <var><b>id</b> 8<br /><b>name</b> Automotive<br /><b>description</b> Automotive</var><br /><br />
&nbsp; <var><b>id</b> 9<br /><b>name</b> Banking<br /><b>description</b> Banking</var><br /><br />
&nbsp; <var><b>id</b> 10<br /><b>name</b> Biotechnology<br /><b>description</b> Biotechnology</var><br /><br />
&nbsp; <var><b>id</b> 11<br /><b>name</b> Broadcasting<br /><b>description</b> Broadcasting</var><br /><br />
&nbsp; <var><b>id</b> 12<br /><b>name</b> Brokerage<br /><b>description</b> Brokerage</var><br /><br />
&nbsp; <var><b>id</b> 13<br /><b>name</b> Business Support & Supplies<br /><b>description</b> Business Support & Supplies</var><br /><br />
&nbsp; <var><b>id</b> 14<br /><b>name</b> Call Centers<br /><b>description</b> Call Centers </var><br /><br />
&nbsp; <var><b>id</b> 15<br /><b>name</b> Cargo Handling<br /><b>description</b> Cargo Handling</var><br /><br />
&nbsp; <var><b>id</b> 16<br /><b>name</b> Chemicals<br /><b>description</b> Chemicals</var><br /><br />
&nbsp; <var><b>id</b> 17<br /><b>name</b> Communications<br /><b>description</b> Communications</var><br /><br />
&nbsp; <var><b>id</b> 18<br /><b>name</b> Computers & Electronics<br /><b>description</b> Computers & Electronics</var><br /><br />
&nbsp; <var><b>id</b> 19<br /><b>name</b> Consumer Products<br /><b>description</b> Consumer Products</var><br /><br />
&nbsp; <var><b>id</b> 20<br /><b>name</b> Cosmetics<br /><b>description</b> Cosmetics</var><br /><br />
&nbsp; <var><b>id</b> 21<br /><b>name</b> Construction<br /><b>description</b> Construction</var><br /><br />
&nbsp; <var><b>id</b> 22<br /><b>name</b> Consulting<br /><b>description</b> Consulting</var><br /><br />
&nbsp; <var><b>id</b> 23<br /><b>name</b> Defense<br /><b>description</b> Defense</var><br /><br />
&nbsp; <var><b>id</b> 24<br /><b>name</b> Department Stores<br /><b>description</b> Department Stores</var><br /><br />
&nbsp; <var><b>id</b> 25<br /><b>name</b> Education<br /><b>description</b> Education</var><br /><br />
&nbsp; <var><b>id</b> 26<br /><b>name</b> Electronics<br /><b>description</b> Electronics</var><br /><br />
&nbsp; <var><b>id</b> 27<br /><b>name</b> Energy<br /><b>description</b> Energy</var><br /><br />
&nbsp; <var><b>id</b> 28<br /><b>name</b> Engineering<br /><b>description</b> Engineering</var><br /><br />
&nbsp; <var><b>id</b> 29<br /><b>name</b> Entertainment<br /><b>description</b> Entertainment</var><br /><br />
&nbsp; <var><b>id</b> 30<br /><b>name</b> Environmental<br /><b>description</b> Environmental</var><br /><br />
&nbsp; <var><b>id</b> 31<br /><b>name</b> Executive Search<br /><b>description</b> Executive Search</var><br /><br />
&nbsp; <var><b>id</b> 32<br /><b>name</b> Finance<br /><b>description</b> Finance</var><br /><br />
&nbsp; <var><b>id</b> 33<br /><b>name</b> Food & Beverage<br /><b>description</b> Food & Beverage</var><br /><br />
&nbsp; <var><b>id</b> 34<br /><b>name</b> Government<br /><b>description</b> Government</var><br /><br />
&nbsp; <var><b>id</b> 35<br /><b>name</b> Grocery<br /><b>description</b> Grocery</var><br /><br />
&nbsp; <var><b>id</b> 36<br /><b>name</b> Healthcare<br /><b>description</b> Healthcare</var><br /><br />
&nbsp; <var><b>id</b> 37<br /><b>name</b> Home & Garden<br /><b>description</b> Home & Garden</var><br /><br />
&nbsp; <var><b>id</b> 38<br /><b>name</b> Hospitality<br /><b>description</b> Hospitality</var><br /><br />
&nbsp; <var><b>id</b> 39<br /><b>name</b> Insurance<br /><b>description</b> Insurance</var><br /><br />
&nbsp; <var><b>id</b> 40<br /><b>name</b> Internet Publishing<br /><b>description</b> Internet Publishing</var><br /><br />
&nbsp; <var><b>id</b> 41<br /><b>name</b> Investment Banking<br /><b>description</b> Investment Banking</var><br /><br />
&nbsp; <var><b>id</b> 42<br /><b>name</b> Legal<br /><b>description</b> Legal</var><br /><br />
&nbsp; <var><b>id</b> 43<br /><b>name</b> Machinery<br /><b>description</b> Machinery</var><br /><br />
&nbsp; <var><b>id</b> 44<br /><b>name</b> Manufacturing<br /><b>description</b> Manufacturing</var><br /><br />
&nbsp; <var><b>id</b> 45<br /><b>name</b> Media<br /><b>description</b> Media</var><br /><br />
&nbsp; <var><b>id</b> 46<br /><b>name</b> Merchants<br /><b>description</b> Merchants</var><br /><br />
&nbsp; <var><b>id</b> 47<br /><b>name</b> Motion Picture & Video<br /><b>description</b> Motion Picture & Video</var><br /><br />
&nbsp; <var><b>id</b> 48<br /><b>name</b> Music<br /><b>description</b> Music</var><br /><br />
&nbsp; <var><b>id</b> 49<br /><b>name</b> Newspaper Publishers<br /><b>description</b> Newspaper Publishers</var><br /><br />
&nbsp; <var><b>id</b> 50<br /><b>name</b> Not For Profit<br /><b>description</b> Not For Profit</var><br /><br />
&nbsp; <var><b>id</b> 51<br /><b>name</b> Online Auctions<br /><b>description</b> Online Auctions</var><br /><br />
&nbsp; <var><b>id</b> 52<br /><b>name</b> Other<br /><b>description</b> Other</var><br /><br />
&nbsp; <var><b>id</b> 53<br /><b>name</b> Pension Funds<br /><b>description</b> Pension Funds</var><br /><br />
&nbsp; <var><b>id</b> 54<br /><b>name</b> Personal Care<br /><b>description</b> Personal Care</var><br /><br />
&nbsp; <var><b>id</b> 55<br /><b>name</b> Pharmaceuticals<br /><b>description</b> Pharmaceuticals</var><br /><br />
&nbsp; <var><b>id</b> 56<br /><b>name</b> Private Equity<br /><b>description</b> Private Equity</var><br /><br />
&nbsp; <var><b>id</b> 57<br /><b>name</b> Publishing<br /><b>description</b> Publishing</var><br /><br />
&nbsp; <var><b>id</b> 58<br /><b>name</b> Real Estate<br /><b>description</b> Real Estate</var><br /><br />
&nbsp; <var><b>id</b> 59<br /><b>name</b> Recreation<br /><b>description</b> Recreation</var><br /><br />
&nbsp; <var><b>id</b> 60<br /><b>name</b> Retail<br /><b>description</b> Retail</var><br /><br />
&nbsp; <var><b>id</b> 61<br /><b>name</b> Securities & Commodity Exchanges<br /><b>description</b> Securities & Commodity Exchanges</var><br /><br />
&nbsp; <var><b>id</b> 62<br /><b>name</b> Service<br /><b>description</b> Service</var><br /><br />
&nbsp; <var><b>id</b> 63<br /><b>name</b> Shipping<br /><b>description</b> Shipping</var><br /><br />
&nbsp; <var><b>id</b> 64<br /><b>name</b> Soap & Detergent<br /><b>description</b> Soap & Detergent</var><br /><br />
&nbsp; <var><b>id</b> 65<br /><b>name</b> Software<br /><b>description</b> Software</var><br /><br />
&nbsp; <var><b>id</b> 66<br /><b>name</b> Technology<br /><b>description</b> Technology</var><br /><br />
&nbsp; <var><b>id</b> 67<br /><b>name</b> Telecommunications<br /><b>description</b> Telecommunications</var><br /><br />
&nbsp; <var><b>id</b> 68<br /><b>name</b> Transportation<br /><b>description</b> Transportation</var><br /><br />
&nbsp; <var><b>id</b> 69<br /><b>name</b> Utilities<br /><b>description</b> Utilities</var><br /><br />
&nbsp; <var><b>id</b> 70<br /><b>name</b> Health and Fitness<br /><b>description</b> Health and Fitness</var><br /><br />
</code>

## Country Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
code | <i class="item-label">string</i><br>| Two letter country code.
country | <i class="item-label">string</i> | Name of the Country

### Possible Countries

<code>
  Countries<br />
&nbsp; <var><b>id</b> 1<br /><b>code</b> AF<br /><b>Country</b> Afghanistan</var><br /><br />
&nbsp; <var><b>id</b> 2<br /><b>code</b> AL<br /><b>Country</b> Albania</var><br /><br />
&nbsp; <var><b>id</b> 3<br /><b>code</b> DZ<br /><b>Country</b> Algeria</var><br /><br />
&nbsp; <var><b>id</b> 4<br /><b>code</b> DS<br /><b>Country</b> American Samoa</var><br /><br />
&nbsp; <var><b>id</b> 5<br /><b>code</b> AD<br /><b>Country</b> Andorra</var><br /><br />
&nbsp; <var><b>id</b> 6<br /><b>code</b> AO<br /><b>Country</b> Angola</var><br /><br />
&nbsp; <var><b>id</b> 7<br /><b>code</b> AI<br /><b>Country</b> Anguilla</var><br /><br />
&nbsp; <var><b>id</b> 8<br /><b>code</b> AQ<br /><b>Country</b> Antarctica</var><br /><br />
&nbsp; <var><b>id</b> 9<br /><b>code</b> AG<br /><b>Country</b> Antigua and Barbuda</var><br /><br />
&nbsp; <var><b>id</b> 10<br /><b>code</b> AR<br /><b>Country</b> Argentina</var><br /><br />
&nbsp; <var><b>id</b> 11<br /><b>code</b> AM<br /><b>Country</b> Armenia</var><br /><br />
&nbsp; <var><b>id</b> 12<br /><b>code</b> AW<br /><b>Country</b> Aruba</var><br /><br />
&nbsp; <var><b>id</b> 13<br /><b>code</b> AU<br /><b>Country</b> Australia</var><br /><br />
&nbsp; <var><b>id</b> 14<br /><b>code</b> AT<br /><b>Country</b> Austria</var><br /><br />
&nbsp; <var><b>id</b> 15<br /><b>code</b> AZ<br /><b>Country</b> Azerbaijan</var><br /><br />
&nbsp; <var><b>id</b> 16<br /><b>code</b> BS<br /><b>Country</b> Bahamas</var><br /><br />
&nbsp; <var><b>id</b> 17<br /><b>code</b> BH<br /><b>Country</b> Bahrain</var><br /><br />
&nbsp; <var><b>id</b> 18<br /><b>code</b> BD<br /><b>Country</b> Bangladesh</var><br /><br />
&nbsp; <var><b>id</b> 19<br /><b>code</b> BB<br /><b>Country</b> Barbados</var><br /><br />
&nbsp; <var><b>id</b> 20<br /><b>code</b> BY<br /><b>Country</b> Belarus</var><br /><br />
&nbsp; <var><b>id</b> 21<br /><b>code</b> BE<br /><b>Country</b> Belgium</var><br /><br />
&nbsp; <var><b>id</b> 22<br /><b>code</b> BZ<br /><b>Country</b> Belize</var><br /><br />
&nbsp; <var><b>id</b> 23<br /><b>code</b> BJ<br /><b>Country</b> Benin</var><br /><br />
&nbsp; <var><b>id</b> 24<br /><b>code</b> BM<br /><b>Country</b> Bermuda</var><br /><br />
&nbsp; <var><b>id</b> 25<br /><b>code</b> BT<br /><b>Country</b> Bhutan</var><br /><br />
&nbsp; <var><b>id</b> 26<br /><b>code</b> BO<br /><b>Country</b> Bolivia</var><br /><br />
&nbsp; <var><b>id</b> 27<br /><b>code</b> BA<br /><b>Country</b> Bosnia and Herzegovina</var><br /><br />
&nbsp; <var><b>id</b> 28<br /><b>code</b> BW<br /><b>Country</b> Botswana</var><br /><br />
&nbsp; <var><b>id</b> 29<br /><b>code</b> BV<br /><b>Country</b> Bouvet Island</var><br /><br />
&nbsp; <var><b>id</b> 30<br /><b>code</b> BR<br /><b>Country</b> Brazil</var><br /><br />
&nbsp; <var><b>id</b> 31<br /><b>code</b> IO<br /><b>Country</b> British Indian Ocean Territory</var><br /><br />
&nbsp; <var><b>id</b> 32<br /><b>code</b> BN<br /><b>Country</b> Brunei Darussalam</var><br /><br />
&nbsp; <var><b>id</b> 33<br /><b>code</b> BG<br /><b>Country</b> Bulgaria</var><br /><br />
&nbsp; <var><b>id</b> 34<br /><b>code</b> BF<br /><b>Country</b> Burkina Faso</var><br /><br />
&nbsp; <var><b>id</b> 35<br /><b>code</b> BI<br /><b>Country</b> Burundi</var><br /><br />
&nbsp; <var><b>id</b> 36<br /><b>code</b> KH<br /><b>Country</b> Cambodia</var><br /><br />
&nbsp; <var><b>id</b> 37<br /><b>code</b> CM<br /><b>Country</b> Cameroon</var><br /><br />
&nbsp; <var><b>id</b> 38<br /><b>code</b> CA<br /><b>Country</b> Canada</var><br /><br />
&nbsp; <var><b>id</b> 39<br /><b>code</b> CV<br /><b>Country</b> Cape Verde</var><br /><br />
&nbsp; <var><b>id</b> 40<br /><b>code</b> KY<br /><b>Country</b> Cayman Islands</var><br /><br />
&nbsp; <var><b>id</b> 41<br /><b>code</b> CF<br /><b>Country</b> Central African Republic</var><br /><br />
&nbsp; <var><b>id</b> 42<br /><b>code</b> TD<br /><b>Country</b> Chad</var><br /><br />
&nbsp; <var><b>id</b> 43<br /><b>code</b> CL<br /><b>Country</b> Chile</var><br /><br />
&nbsp; <var><b>id</b> 44<br /><b>code</b> CN<br /><b>Country</b> China</var><br /><br />
&nbsp; <var><b>id</b> 45<br /><b>code</b> CX<br /><b>Country</b> Christmas Island</var><br /><br />
&nbsp; <var><b>id</b> 46<br /><b>code</b> CC<br /><b>Country</b> Cocos (Keeling) Islands</var><br /><br />
&nbsp; <var><b>id</b> 47<br /><b>code</b> CO<br /><b>Country</b> Colombia</var><br /><br />
&nbsp; <var><b>id</b> 48<br /><b>code</b> KM<br /><b>Country</b> Comoros</var><br /><br />
&nbsp; <var><b>id</b> 49<br /><b>code</b> CG<br /><b>Country</b> Congo</var><br /><br />
&nbsp; <var><b>id</b> 50<br /><b>code</b> CK<br /><b>Country</b> Cook Islands</var><br /><br />
&nbsp; <var><b>id</b> 51<br /><b>code</b> CR<br /><b>Country</b> Costa Rica</var><br /><br />
&nbsp; <var><b>id</b> 52<br /><b>code</b> HR<br /><b>Country</b> Croatia (Hrvatska)</var><br /><br />
&nbsp; <var><b>id</b> 53<br /><b>code</b> CU<br /><b>Country</b> Cuba</var><br /><br />
&nbsp; <var><b>id</b> 54<br /><b>code</b> CY<br /><b>Country</b> Cyprus</var><br /><br />
&nbsp; <var><b>id</b> 55<br /><b>code</b> CZ<br /><b>Country</b> Czech Republic</var><br /><br />
&nbsp; <var><b>id</b> 56<br /><b>code</b> DK<br /><b>Country</b> Denmark</var><br /><br />
&nbsp; <var><b>id</b> 57<br /><b>code</b> DJ<br /><b>Country</b> Djibouti</var><br /><br />
&nbsp; <var><b>id</b> 58<br /><b>code</b> DM<br /><b>Country</b> Dominica</var><br /><br />
&nbsp; <var><b>id</b> 59<br /><b>code</b> DO<br /><b>Country</b> Dominican Republic</var><br /><br />
&nbsp; <var><b>id</b> 60<br /><b>code</b> TP<br /><b>Country</b> East Timor</var><br /><br />
&nbsp; <var><b>id</b> 61<br /><b>code</b> EC<br /><b>Country</b> Ecuador</var><br /><br />
&nbsp; <var><b>id</b> 62<br /><b>code</b> EG<br /><b>Country</b> Egypt</var><br /><br />
&nbsp; <var><b>id</b> 63<br /><b>code</b> SV<br /><b>Country</b> El Salvador</var><br /><br />
&nbsp; <var><b>id</b> 64<br /><b>code</b> GQ<br /><b>Country</b> Equatorial Guinea</var><br /><br />
&nbsp; <var><b>id</b> 65<br /><b>code</b> ER<br /><b>Country</b> Eritrea</var><br /><br />
&nbsp; <var><b>id</b> 66<br /><b>code</b> EE<br /><b>Country</b> Estonia</var><br /><br />
&nbsp; <var><b>id</b> 67<br /><b>code</b> ET<br /><b>Country</b> Ethiopia</var><br /><br />
&nbsp; <var><b>id</b> 68<br /><b>code</b> FK<br /><b>Country</b> Falkland Islands (Malvinas)</var><br /><br />
&nbsp; <var><b>id</b> 69<br /><b>code</b> FO<br /><b>Country</b> Faroe Islands</var><br /><br />
&nbsp; <var><b>id</b> 70<br /><b>code</b> FJ<br /><b>Country</b> Fiji</var><br /><br />
&nbsp; <var><b>id</b> 71<br /><b>code</b> FI<br /><b>Country</b> Finland</var><br /><br />
&nbsp; <var><b>id</b> 72<br /><b>code</b> FR<br /><b>Country</b> France</var><br /><br />
&nbsp; <var><b>id</b> 73<br /><b>code</b> FX<br /><b>Country</b> France, Metropolitan</var><br /><br />
&nbsp; <var><b>id</b> 74<br /><b>code</b> GF<br /><b>Country</b> French Guiana</var><br /><br />
&nbsp; <var><b>id</b> 75<br /><b>code</b> PF<br /><b>Country</b> French Polynesia</var><br /><br />
&nbsp; <var><b>id</b> 76<br /><b>code</b> TF<br /><b>Country</b> French Southern Territories</var><br /><br />
&nbsp; <var><b>id</b> 77<br /><b>code</b> GA<br /><b>Country</b> Gabon</var><br /><br />
&nbsp; <var><b>id</b> 78<br /><b>code</b> GM<br /><b>Country</b> Gambia</var><br /><br />
&nbsp; <var><b>id</b> 79<br /><b>code</b> GE<br /><b>Country</b> Georgia</var><br /><br />
&nbsp; <var><b>id</b> 80<br /><b>code</b> DE<br /><b>Country</b> Germany</var><br /><br />
&nbsp; <var><b>id</b> 81<br /><b>code</b> GH<br /><b>Country</b> Ghana</var><br /><br />
&nbsp; <var><b>id</b> 82<br /><b>code</b> GI<br /><b>Country</b> Gibraltar</var><br /><br />
&nbsp; <var><b>id</b> 83<br /><b>code</b> GK<br /><b>Country</b> Guernsey</var><br /><br />
&nbsp; <var><b>id</b> 84<br /><b>code</b> GR<br /><b>Country</b> Greece</var><br /><br />
&nbsp; <var><b>id</b> 85<br /><b>code</b> GL<br /><b>Country</b> Greenland</var><br /><br />
&nbsp; <var><b>id</b> 86<br /><b>code</b> GD<br /><b>Country</b> Grenada</var><br /><br />
&nbsp; <var><b>id</b> 87<br /><b>code</b> GP<br /><b>Country</b> Guadeloupe</var><br /><br />
&nbsp; <var><b>id</b> 88<br /><b>code</b> GU<br /><b>Country</b> Guam</var><br /><br />
&nbsp; <var><b>id</b> 89<br /><b>code</b> GT<br /><b>Country</b> Guatemala</var><br /><br />
&nbsp; <var><b>id</b> 90<br /><b>code</b> GN<br /><b>Country</b> Guinea</var><br /><br />
&nbsp; <var><b>id</b> 91<br /><b>code</b> GW<br /><b>Country</b> Guinea-Bissau</var><br /><br />
&nbsp; <var><b>id</b> 92<br /><b>code</b> GY<br /><b>Country</b> Guyana</var><br /><br />
&nbsp; <var><b>id</b> 93<br /><b>code</b> HT<br /><b>Country</b> Haiti</var><br /><br />
&nbsp; <var><b>id</b> 94<br /><b>code</b> HM<br /><b>Country</b> Heard and Mc Donald Islands</var><br /><br />
&nbsp; <var><b>id</b> 95<br /><b>code</b> HN<br /><b>Country</b> Honduras</var><br /><br />
&nbsp; <var><b>id</b> 96<br /><b>code</b> HK<br /><b>Country</b> Hong Kong</var><br /><br />
&nbsp; <var><b>id</b> 97<br /><b>code</b> HU<br /><b>Country</b> Hungary</var><br /><br />
&nbsp; <var><b>id</b> 98<br /><b>code</b> IS<br /><b>Country</b> Iceland</var><br /><br />
&nbsp; <var><b>id</b> 99<br /><b>code</b> IN<br /><b>Country</b> India</var><br /><br />
&nbsp; <var><b>id</b> 100<br /><b>code</b> IM<br /><b>Country</b> Isle of Man  	 </var><br /><br />
&nbsp; <var><b>id</b> 101<br /><b>code</b> ID<br /><b>Country</b> Indonesia</var><br /><br />
&nbsp; <var><b>id</b> 102<br /><b>code</b> IR<br /><b>Country</b> Iran (Islamic Republic of)</var><br /><br />
&nbsp; <var><b>id</b> 103<br /><b>code</b> IQ<br /><b>Country</b> Iraq</var><br /><br />
&nbsp; <var><b>id</b> 104<br /><b>code</b> IE<br /><b>Country</b> Ireland</var><br /><br />
&nbsp; <var><b>id</b> 105<br /><b>code</b> IL<br /><b>Country</b> Israel</var><br /><br />
&nbsp; <var><b>id</b> 106<br /><b>code</b> IT<br /><b>Country</b> Italy</var><br /><br />
&nbsp; <var><b>id</b> 107<br /><b>code</b> CI<br /><b>Country</b> Ivory Coast</var><br /><br />
&nbsp; <var><b>id</b> 108<br /><b>code</b> JE<br /><b>Country</b> Jersey</var><br /><br />
&nbsp; <var><b>id</b> 109<br /><b>code</b> JM<br /><b>Country</b> Jamaica</var><br /><br />
&nbsp; <var><b>id</b> 110<br /><b>code</b> JP<br /><b>Country</b> Japan</var><br /><br />
&nbsp; <var><b>id</b> 111<br /><b>code</b> JO<br /><b>Country</b> Jordan</var><br /><br />
&nbsp; <var><b>id</b> 112<br /><b>code</b> KZ<br /><b>Country</b> Kazakhstan</var><br /><br />
&nbsp; <var><b>id</b> 113<br /><b>code</b> KE<br /><b>Country</b> Kenya</var><br /><br />
&nbsp; <var><b>id</b> 114<br /><b>code</b> KI<br /><b>Country</b> Kiribati</var><br /><br />
&nbsp; <var><b>id</b> 115<br /><b>code</b> KP<br /><b>Country</b> Korea, Democratic People's Republic of</var><br /><br />
&nbsp; <var><b>id</b> 116<br /><b>code</b> KR<br /><b>Country</b> Korea, Republic of</var><br /><br />
&nbsp; <var><b>id</b> 117<br /><b>code</b> XK<br /><b>Country</b> Kosovo</var><br /><br />
&nbsp; <var><b>id</b> 118<br /><b>code</b> KW<br /><b>Country</b> Kuwait</var><br /><br />
&nbsp; <var><b>id</b> 119<br /><b>code</b> KG<br /><b>Country</b> Kyrgyzstan</var><br /><br />
&nbsp; <var><b>id</b> 120<br /><b>code</b> LA<br /><b>Country</b> Lao People's Democratic Republic</var><br /><br />
&nbsp; <var><b>id</b> 121<br /><b>code</b> LV<br /><b>Country</b> Latvia</var><br /><br />
&nbsp; <var><b>id</b> 122<br /><b>code</b> LB<br /><b>Country</b> Lebanon</var><br /><br />
&nbsp; <var><b>id</b> 123<br /><b>code</b> LS<br /><b>Country</b> Lesotho</var><br /><br />
&nbsp; <var><b>id</b> 124<br /><b>code</b> LR<br /><b>Country</b> Liberia</var><br /><br />
&nbsp; <var><b>id</b> 125<br /><b>code</b> LY<br /><b>Country</b> Libyan Arab Jamahiriya</var><br /><br />
&nbsp; <var><b>id</b> 126<br /><b>code</b> LI<br /><b>Country</b> Liechtenstein</var><br /><br />
&nbsp; <var><b>id</b> 127<br /><b>code</b> LT<br /><b>Country</b> Lithuania</var><br /><br />
&nbsp; <var><b>id</b> 128<br /><b>code</b> LU<br /><b>Country</b> Luxembourg</var><br /><br />
&nbsp; <var><b>id</b> 129<br /><b>code</b> MO<br /><b>Country</b> Macau</var><br /><br />
&nbsp; <var><b>id</b> 130<br /><b>code</b> MK<br /><b>Country</b> Macedonia</var><br /><br />
&nbsp; <var><b>id</b> 131<br /><b>code</b> MG<br /><b>Country</b> Madagascar</var><br /><br />
&nbsp; <var><b>id</b> 132<br /><b>code</b> MW<br /><b>Country</b> Malawi</var><br /><br />
&nbsp; <var><b>id</b> 133<br /><b>code</b> MY<br /><b>Country</b> Malaysia</var><br /><br />
&nbsp; <var><b>id</b> 134<br /><b>code</b> MV<br /><b>Country</b> Maldives</var><br /><br />
&nbsp; <var><b>id</b> 135<br /><b>code</b> ML<br /><b>Country</b> Mali</var><br /><br />
&nbsp; <var><b>id</b> 136<br /><b>code</b> MT<br /><b>Country</b> Malta</var><br /><br />
&nbsp; <var><b>id</b> 137<br /><b>code</b> MH<br /><b>Country</b> Marshall Islands</var><br /><br />
&nbsp; <var><b>id</b> 138<br /><b>code</b> MQ<br /><b>Country</b> Martinique</var><br /><br />
&nbsp; <var><b>id</b> 139<br /><b>code</b> MR<br /><b>Country</b> Mauritania</var><br /><br />
&nbsp; <var><b>id</b> 140<br /><b>code</b> MU<br /><b>Country</b> Mauritius</var><br /><br />
&nbsp; <var><b>id</b> 141<br /><b>code</b> TY<br /><b>Country</b> Mayotte</var><br /><br />
&nbsp; <var><b>id</b> 142<br /><b>code</b> MX<br /><b>Country</b> Mexico</var><br /><br />
&nbsp; <var><b>id</b> 143<br /><b>code</b> FM<br /><b>Country</b> Micronesia, Federated States of</var><br /><br />
&nbsp; <var><b>id</b> 144<br /><b>code</b> MD<br /><b>Country</b> Moldova, Republic of</var><br /><br />
&nbsp; <var><b>id</b> 145<br /><b>code</b> MC<br /><b>Country</b> Monaco</var><br /><br />
&nbsp; <var><b>id</b> 146<br /><b>code</b> MN<br /><b>Country</b> Mongolia</var><br /><br />
&nbsp; <var><b>id</b> 147<br /><b>code</b> ME<br /><b>Country</b> Montenegro</var><br /><br />
&nbsp; <var><b>id</b> 148<br /><b>code</b> MS<br /><b>Country</b> Montserrat</var><br /><br />
&nbsp; <var><b>id</b> 149<br /><b>code</b> MA<br /><b>Country</b> Morocco</var><br /><br />
&nbsp; <var><b>id</b> 150<br /><b>code</b> MZ<br /><b>Country</b> Mozambique</var><br /><br />
&nbsp; <var><b>id</b> 151<br /><b>code</b> MM<br /><b>Country</b> Myanmar</var><br /><br />
&nbsp; <var><b>id</b> 152<br /><b>code</b> NA<br /><b>Country</b> Namibia</var><br /><br />
&nbsp; <var><b>id</b> 153<br /><b>code</b> NR<br /><b>Country</b> Nauru</var><br /><br />
&nbsp; <var><b>id</b> 154<br /><b>code</b> NP<br /><b>Country</b> Nepal</var><br /><br />
&nbsp; <var><b>id</b> 155<br /><b>code</b> NL<br /><b>Country</b> Netherlands</var><br /><br />
&nbsp; <var><b>id</b> 156<br /><b>code</b> AN<br /><b>Country</b> Netherlands Antilles</var><br /><br />
&nbsp; <var><b>id</b> 157<br /><b>code</b> NC<br /><b>Country</b> New Caledonia</var><br /><br />
&nbsp; <var><b>id</b> 158<br /><b>code</b> NZ<br /><b>Country</b> New Zealand</var><br /><br />
&nbsp; <var><b>id</b> 159<br /><b>code</b> NI<br /><b>Country</b> Nicaragua</var><br /><br />
&nbsp; <var><b>id</b> 160<br /><b>code</b> NE<br /><b>Country</b> Niger</var><br /><br />
&nbsp; <var><b>id</b> 161<br /><b>code</b> NG<br /><b>Country</b> Nigeria</var><br /><br />
&nbsp; <var><b>id</b> 162<br /><b>code</b> NU<br /><b>Country</b> Niue</var><br /><br />
&nbsp; <var><b>id</b> 163<br /><b>code</b> NF<br /><b>Country</b> Norfolk Island</var><br /><br />
&nbsp; <var><b>id</b> 164<br /><b>code</b> MP<br /><b>Country</b> Northern Mariana Islands</var><br /><br />
&nbsp; <var><b>id</b> 165<br /><b>code</b> NO<br /><b>Country</b> Norway</var><br /><br />
&nbsp; <var><b>id</b> 166<br /><b>code</b> OM<br /><b>Country</b> Oman</var><br /><br />
&nbsp; <var><b>id</b> 167<br /><b>code</b> PK<br /><b>Country</b> Pakistan</var><br /><br />
&nbsp; <var><b>id</b> 168<br /><b>code</b> PW<br /><b>Country</b> Palau</var><br /><br />
&nbsp; <var><b>id</b> 169<br /><b>code</b> PS<br /><b>Country</b> Palestine</var><br /><br />
&nbsp; <var><b>id</b> 170<br /><b>code</b> PA<br /><b>Country</b> Panama</var><br /><br />
&nbsp; <var><b>id</b> 171<br /><b>code</b> PG<br /><b>Country</b> Papua New Guinea</var><br /><br />
&nbsp; <var><b>id</b> 172<br /><b>code</b> PY<br /><b>Country</b> Paraguay</var><br /><br />
&nbsp; <var><b>id</b> 173<br /><b>code</b> PE<br /><b>Country</b> Peru</var><br /><br />
&nbsp; <var><b>id</b> 174<br /><b>code</b> PH<br /><b>Country</b> Philippines</var><br /><br />
&nbsp; <var><b>id</b> 175<br /><b>code</b> PN<br /><b>Country</b> Pitcairn</var><br /><br />
&nbsp; <var><b>id</b> 176<br /><b>code</b> PL<br /><b>Country</b> Poland</var><br /><br />
&nbsp; <var><b>id</b> 177<br /><b>code</b> PT<br /><b>Country</b> Portugal</var><br /><br />
&nbsp; <var><b>id</b> 178<br /><b>code</b> PR<br /><b>Country</b> Puerto Rico</var><br /><br />
&nbsp; <var><b>id</b> 179<br /><b>code</b> QA<br /><b>Country</b> Qatar</var><br /><br />
&nbsp; <var><b>id</b> 180<br /><b>code</b> RE<br /><b>Country</b> Reunion</var><br /><br />
&nbsp; <var><b>id</b> 181<br /><b>code</b> RO<br /><b>Country</b> Romania</var><br /><br />
&nbsp; <var><b>id</b> 182<br /><b>code</b> RU<br /><b>Country</b> Russian Federation</var><br /><br />
&nbsp; <var><b>id</b> 183<br /><b>code</b> RW<br /><b>Country</b> Rwanda</var><br /><br />
&nbsp; <var><b>id</b> 184<br /><b>code</b> KN<br /><b>Country</b> Saint Kitts and Nevis</var><br /><br />
&nbsp; <var><b>id</b> 185<br /><b>code</b> LC<br /><b>Country</b> Saint Lucia</var><br /><br />
&nbsp; <var><b>id</b> 186<br /><b>code</b> VC<br /><b>Country</b> Saint Vincent and the Grenadines</var><br /><br />
&nbsp; <var><b>id</b> 187<br /><b>code</b> WS<br /><b>Country</b> Samoa</var><br /><br />
&nbsp; <var><b>id</b> 188<br /><b>code</b> SM<br /><b>Country</b> San Marino</var><br /><br />
&nbsp; <var><b>id</b> 189<br /><b>code</b> ST<br /><b>Country</b> Sao Tome and Principe</var><br /><br />
&nbsp; <var><b>id</b> 190<br /><b>code</b> SA<br /><b>Country</b> Saudi Arabia</var><br /><br />
&nbsp; <var><b>id</b> 191<br /><b>code</b> SN<br /><b>Country</b> Senegal</var><br /><br />
&nbsp; <var><b>id</b> 192<br /><b>code</b> RS<br /><b>Country</b> Serbia</var><br /><br />
&nbsp; <var><b>id</b> 193<br /><b>code</b> SC<br /><b>Country</b> Seychelles</var><br /><br />
&nbsp; <var><b>id</b> 194<br /><b>code</b> SL<br /><b>Country</b> Sierra Leone</var><br /><br />
&nbsp; <var><b>id</b> 195<br /><b>code</b> SG<br /><b>Country</b> Singapore</var><br /><br />
&nbsp; <var><b>id</b> 196<br /><b>code</b> SK<br /><b>Country</b> Slovakia</var><br /><br />
&nbsp; <var><b>id</b> 197<br /><b>code</b> SI<br /><b>Country</b> Slovenia</var><br /><br />
&nbsp; <var><b>id</b> 198<br /><b>code</b> SB<br /><b>Country</b> Solomon Islands</var><br /><br />
&nbsp; <var><b>id</b> 199<br /><b>code</b> SO<br /><b>Country</b> Somalia</var><br /><br />
&nbsp; <var><b>id</b> 200<br /><b>code</b> ZA<br /><b>Country</b> South Africa  	 </var><br /><br />
&nbsp; <var><b>id</b> 201<br /><b>code</b> GS<br /><b>Country</b> South Georgia South Sandwich Islands</var><br /><br />
&nbsp; <var><b>id</b> 202<br /><b>code</b> ES<br /><b>Country</b> Spain</var><br /><br />
&nbsp; <var><b>id</b> 203<br /><b>code</b> LK<br /><b>Country</b> Sri Lanka</var><br /><br />
&nbsp; <var><b>id</b> 204<br /><b>code</b> SH<br /><b>Country</b> St. Helena</var><br /><br />
&nbsp; <var><b>id</b> 205<br /><b>code</b> PM<br /><b>Country</b> St. Pierre and Miquelon</var><br /><br />
&nbsp; <var><b>id</b> 206<br /><b>code</b> SD<br /><b>Country</b> Sudan</var><br /><br />
&nbsp; <var><b>id</b> 207<br /><b>code</b> SR<br /><b>Country</b> Suriname</var><br /><br />
&nbsp; <var><b>id</b> 208<br /><b>code</b> SJ<br /><b>Country</b> Svalbard and Jan Mayen Islands</var><br /><br />
&nbsp; <var><b>id</b> 209<br /><b>code</b> SZ<br /><b>Country</b> Swaziland</var><br /><br />
&nbsp; <var><b>id</b> 210<br /><b>code</b> SE<br /><b>Country</b> Sweden</var><br /><br />
&nbsp; <var><b>id</b> 211<br /><b>code</b> CH<br /><b>Country</b> Switzerland</var><br /><br />
&nbsp; <var><b>id</b> 212<br /><b>code</b> SY<br /><b>Country</b> Syrian Arab Republic</var><br /><br />
&nbsp; <var><b>id</b> 213<br /><b>code</b> TW<br /><b>Country</b> Taiwan</var><br /><br />
&nbsp; <var><b>id</b> 214<br /><b>code</b> TJ<br /><b>Country</b> Tajikistan</var><br /><br />
&nbsp; <var><b>id</b> 215<br /><b>code</b> TZ<br /><b>Country</b> Tanzania, United Republic of</var><br /><br />
&nbsp; <var><b>id</b> 216<br /><b>code</b> TH<br /><b>Country</b> Thailand</var><br /><br />
&nbsp; <var><b>id</b> 217<br /><b>code</b> TG<br /><b>Country</b> Togo</var><br /><br />
&nbsp; <var><b>id</b> 218<br /><b>code</b> TK<br /><b>Country</b> Tokelau</var><br /><br />
&nbsp; <var><b>id</b> 219<br /><b>code</b> TO<br /><b>Country</b> Tonga</var><br /><br />
&nbsp; <var><b>id</b> 220<br /><b>code</b> TT<br /><b>Country</b> Trinidad and Tobago</var><br /><br />
&nbsp; <var><b>id</b> 221<br /><b>code</b> TN<br /><b>Country</b> Tunisia</var><br /><br />
&nbsp; <var><b>id</b> 222<br /><b>code</b> TR<br /><b>Country</b> Turkey</var><br /><br />
&nbsp; <var><b>id</b> 223<br /><b>code</b> TM<br /><b>Country</b> Turkmenistan</var><br /><br />
&nbsp; <var><b>id</b> 224<br /><b>code</b> TC<br /><b>Country</b> Turks and Caicos Islands</var><br /><br />
&nbsp; <var><b>id</b> 225<br /><b>code</b> TV<br /><b>Country</b> Tuvalu</var><br /><br />
&nbsp; <var><b>id</b> 226<br /><b>code</b> UG<br /><b>Country</b> Uganda</var><br /><br />
&nbsp; <var><b>id</b> 227<br /><b>code</b> UA<br /><b>Country</b> Ukraine</var><br /><br />
&nbsp; <var><b>id</b> 228<br /><b>code</b> AE<br /><b>Country</b> United Arab Emirates</var><br /><br />
&nbsp; <var><b>id</b> 229<br /><b>code</b> GB<br /><b>Country</b> United Kingdom</var><br /><br />
&nbsp; <var><b>id</b> 230<br /><b>code</b> US<br /><b>Country</b> United States</var><br /><br />
&nbsp; <var><b>id</b> 231<br /><b>code</b> UM<br /><b>Country</b> United States minor outlying islands</var><br /><br />
&nbsp; <var><b>id</b> 232<br /><b>code</b> UY<br /><b>Country</b> Uruguay</var><br /><br />
&nbsp; <var><b>id</b> 233<br /><b>code</b> UZ<br /><b>Country</b> Uzbekistan</var><br /><br />
&nbsp; <var><b>id</b> 234<br /><b>code</b> VU<br /><b>Country</b> Vanuatu</var><br /><br />
&nbsp; <var><b>id</b> 235<br /><b>code</b> VA<br /><b>Country</b> Vatican City State</var><br /><br />
&nbsp; <var><b>id</b> 236<br /><b>code</b> VE<br /><b>Country</b> Venezuela</var><br /><br />
&nbsp; <var><b>id</b> 237<br /><b>code</b> VN<br /><b>Country</b> Vietnam</var><br /><br />
&nbsp; <var><b>id</b> 238<br /><b>code</b> VG<br /><b>Country</b> Virgin Islands (British)</var><br /><br />
&nbsp; <var><b>id</b> 239<br /><b>code</b> VI<br /><b>Country</b> Virgin Islands (U.S.)</var><br /><br />
&nbsp; <var><b>id</b> 240<br /><b>code</b> WF<br /><b>Country</b> Wallis and Futuna Islands</var><br /><br />
&nbsp; <var><b>id</b> 241<br /><b>code</b> EH<br /><b>Country</b> Western Sahara</var><br /><br />
&nbsp; <var><b>id</b> 242<br /><b>code</b> YE<br /><b>Country</b> Yemen</var><br /><br />
&nbsp; <var><b>id</b> 243<br /><b>code</b> ZR<br /><b>Country</b> Zaire</var><br /><br />
&nbsp; <var><b>id</b> 244<br /><b>code</b> ZM<br /><b>Country</b> Zambia</var><br /><br />
&nbsp; <var><b>id</b> 245<br /><b>code</b> ZW<br /><b>Country</b> Zimbabwe</var><br /><br />
</code>

## State Object

Attribute |   | Description
--------- | - | -----------
id | <i class="item-label">integer</i> | Internal unique identifier for the object.
name | <i class="item-label">string</i><br>| Name of the state.
abbr | <i class="item-label">string</i> | Two letter United States state code.

### Possible States

<code>
  States<br />
&nbsp; <var><b>id</b> 1<br /><b>name</b> Alabama<br /><b>abbr</b> AL</var><br /><br />
&nbsp; <var><b>id</b> 2<br /><b>name</b> Alaska<br /><b>abbr</b> AK</var><br /><br />
&nbsp; <var><b>id</b> 3<br /><b>name</b> Arizona<br /><b>abbr</b> AZ</var><br /><br />
&nbsp; <var><b>id</b> 4<br /><b>name</b> Arkansas<br /><b>abbr</b> AR</var><br /><br />
&nbsp; <var><b>id</b> 5<br /><b>name</b> California<br /><b>abbr</b> CA</var><br /><br />
&nbsp; <var><b>id</b> 6<br /><b>name</b> Colorado<br /><b>abbr</b> CO</var><br /><br />
&nbsp; <var><b>id</b> 7<br /><b>name</b> Connecticut<br /><b>abbr</b> CT</var><br /><br />
&nbsp; <var><b>id</b> 8<br /><b>name</b> Delaware<br /><b>abbr</b> DE</var><br /><br />
&nbsp; <var><b>id</b> 9<br /><b>name</b> Florida<br /><b>abbr</b> FL</var><br /><br />
&nbsp; <var><b>id</b> 10<br /><b>name</b> Georgia<br /><b>abbr</b> GA</var><br /><br />
&nbsp; <var><b>id</b> 11<br /><b>name</b> Hawaii<br /><b>abbr</b> HI</var><br /><br />
&nbsp; <var><b>id</b> 12<br /><b>name</b> Idaho<br /><b>abbr</b> ID</var><br /><br />
&nbsp; <var><b>id</b> 13<br /><b>name</b> Illinois<br /><b>abbr</b> IL</var><br /><br />
&nbsp; <var><b>id</b> 14<br /><b>name</b> Indiana<br /><b>abbr</b> IN</var><br /><br />
&nbsp; <var><b>id</b> 15<br /><b>name</b> Iowa<br /><b>abbr</b> IA</var><br /><br />
&nbsp; <var><b>id</b> 16<br /><b>name</b> Kansas<br /><b>abbr</b> KS</var><br /><br />
&nbsp; <var><b>id</b> 17<br /><b>name</b> Kentucky<br /><b>abbr</b> KY</var><br /><br />
&nbsp; <var><b>id</b> 18<br /><b>name</b> Louisiana<br /><b>abbr</b> LA</var><br /><br />
&nbsp; <var><b>id</b> 19<br /><b>name</b> Maine<br /><b>abbr</b> ME</var><br /><br />
&nbsp; <var><b>id</b> 20<br /><b>name</b> Maryland<br /><b>abbr</b> MD</var><br /><br />
&nbsp; <var><b>id</b> 21<br /><b>name</b> Massachusetts<br /><b>abbr</b> MA</var><br /><br />
&nbsp; <var><b>id</b> 22<br /><b>name</b> Michigan<br /><b>abbr</b> MI</var><br /><br />
&nbsp; <var><b>id</b> 23<br /><b>name</b> Minnesota<br /><b>abbr</b> MN</var><br /><br />
&nbsp; <var><b>id</b> 24<br /><b>name</b> Mississippi<br /><b>abbr</b> MS</var><br /><br />
&nbsp; <var><b>id</b> 25<br /><b>name</b> Missouri<br /><b>abbr</b> MO</var><br /><br />
&nbsp; <var><b>id</b> 26<br /><b>name</b> Montana<br /><b>abbr</b> MT</var><br /><br />
&nbsp; <var><b>id</b> 27<br /><b>name</b> Nebraska<br /><b>abbr</b> NE</var><br /><br />
&nbsp; <var><b>id</b> 28<br /><b>name</b> Nevada<br /><b>abbr</b> NV</var><br /><br />
&nbsp; <var><b>id</b> 29<br /><b>name</b> New Hampshire<br /><b>abbr</b> NH</var><br /><br />
&nbsp; <var><b>id</b> 30<br /><b>name</b> New Jersey<br /><b>abbr</b> NJ</var><br /><br />
&nbsp; <var><b>id</b> 31<br /><b>name</b> New Mexico<br /><b>abbr</b> NM</var><br /><br />
&nbsp; <var><b>id</b> 32<br /><b>name</b> New York<br /><b>abbr</b> NY</var><br /><br />
&nbsp; <var><b>id</b> 33<br /><b>name</b> North Carolina<br /><b>abbr</b> NC</var><br /><br />
&nbsp; <var><b>id</b> 34<br /><b>name</b> North Dakota<br /><b>abbr</b> ND</var><br /><br />
&nbsp; <var><b>id</b> 35<br /><b>name</b> Ohio<br /><b>abbr</b> OH</var><br /><br />
&nbsp; <var><b>id</b> 36<br /><b>name</b> Oklahoma<br /><b>abbr</b> OK</var><br /><br />
&nbsp; <var><b>id</b> 37<br /><b>name</b> Oregon<br /><b>abbr</b> OR</var><br /><br />
&nbsp; <var><b>id</b> 38<br /><b>name</b> Pennsylvania<br /><b>abbr</b> PA</var><br /><br />
&nbsp; <var><b>id</b> 39<br /><b>name</b> Rhode Island<br /><b>abbr</b> RI</var><br /><br />
&nbsp; <var><b>id</b> 40<br /><b>name</b> South Carolina<br /><b>abbr</b> SC</var><br /><br />
&nbsp; <var><b>id</b> 41<br /><b>name</b> South Dakota<br /><b>abbr</b> SD</var><br /><br />
&nbsp; <var><b>id</b> 42<br /><b>name</b> Tennessee<br /><b>abbr</b> TN</var><br /><br />
&nbsp; <var><b>id</b> 43<br /><b>name</b> Texas<br /><b>abbr</b> TX</var><br /><br />
&nbsp; <var><b>id</b> 44<br /><b>name</b> Utah<br /><b>abbr</b> UT</var><br /><br />
&nbsp; <var><b>id</b> 45<br /><b>name</b> Vermont<br /><b>abbr</b> VT</var><br /><br />
&nbsp; <var><b>id</b> 46<br /><b>name</b> Virginia<br /><b>abbr</b> VA</var><br /><br />
&nbsp; <var><b>id</b> 47<br /><b>name</b> Washington<br /><b>abbr</b> WA</var><br /><br />
&nbsp; <var><b>id</b> 48<br /><b>name</b> West Virginia<br /><b>abbr</b> WV</var><br /><br />
&nbsp; <var><b>id</b> 49<br /><b>name</b> Wisconsin<br /><b>abbr</b> WI</var><br /><br />
&nbsp; <var><b>id</b> 50<br /><b>name</b> Wyoming WY </var><br /><br />
</code>

## Retrieve A Business List

> <b>GET /api/v1/businesses</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/businesses"
  -u "<API_TOKEN>"
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
{
    "brands": [
        {...}
    ]
}
```

```php
{
    "brands": [
        {...}
    ]
}
```

```ruby
{
    "brands": [
        {...}
    ]
}
```

```python
{
    "brands": [
        {...}
    ]
}
```

```go
{
    "brands": [
        {...}
    ]
}
```

```javascript
{
    "brands": [
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a list of accessible brands.

### HTTP Request

`GET https://dev.qebot.com/api/v1/brands`

### Returns
 Returns an array of businesses.

## Create Business

> <b>POST /api/v1/businesses</b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/businesses"
  -X POST
  -u "<API_TOKEN>"
  -d business_name="Business Name"
  -d category_id=1
  -d phone=1234567890
  -d fax=1234567890
  -d address="123 fake st"
  -d address2="Suite #2"
  -d city="San Francisco"
  -d state_id=1
  -d country_id=1
  -d zipcode=12345
  -d email=user@example.com
  -d website="http://example.com"
  -d status=active
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
{
    "businesses":[
        {...}
    ]
}
```

```php
{
    "businesses":[
        {...}
    ]
}
```

```ruby
{
    "businesses":[
        {...}
    ]
}
```

```python
{
    "businesses":[
        {...}
    ]
}
```

```go
{
    "businesses":[
        {...}
    ]
}
```

```javascript
{
    "businesses":[
        {...}
    ]
}
```

<span title="post" class="pg-type type-post">post</span>

Create a new business.

### HTTP Request

`POST https://dev.qebot.com/api/v1/businesses`

<aside class="notice">
The dot notation indicates that the property is one level deep inside a hash.<br />
The `[]` indicates the property is an array of objects
</aside>
<h5 class="sidebar-nav-heading">Request Arguments</h5>

Attribute |   | Description
--------- | - | -----------
business_name | <i class="item-label">string</i><var>required</var>| Name of the business.
brand_id | <i class="item-label">integer</i><var>required</var> | Unique identifier of brand associated with the business.
category_id | <i class="item-label">integer</i><var>required</var> | Identifier for what category a business belongs to.  See [Category](#category-object) object
phone  | <i class="item-label">string</i>| A phone contact number of the busieness.
fax  | <i class="item-label">string</i> | A fax number for the busieness.
address  | <i class="item-label">string</i><var>required</var>| Address of the business.
address2  | <i class="item-label">string</i> | Extra information for business address.
city  | <i class="item-label">string</i><var>required</var>| City of the business.
state_id  | <i class="item-label">integer</i> | Extra information State identifier for the business. See [State](#state-object) object
state_name  | <i class="item-label">string</i> | Name of the state where address resides.
country_id  | <i class="item-label">integer</i><var>required</var>| Country identifier for the business. See [Country](#country-object) object
zipcode  | <i class="item-label">string</i><var>required</var>| Zipcode of the business.
email  | <i class="item-label">string</i><var>required</var>| Contact email for the business.
website  | <i class="item-label">string</i>| Website for the business.
status  | <i class="item-label">string</i><var>required</var>| Status of the business.<br />Possible values: (<b>active</b>, <b>inactive</b>)

### Returns
 Returns an array of a business.

## Retrieve Business

> <b>GET /api/v1/brands/ <var>id</var></b>

> Example Request

 ```shell
# With shell, you can just pass the correct header with each request
curl "https://dev.qebot.com/api/v1/brands/<ID>"
  -u "<API_TOKEN>"
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
{
    "businesses": [
        {...}
    ]
}
```

```php
{
    "businesses": [
        {...}
    ]
}
```

```ruby
{
    "businesses": [
        {...}
    ]
}
```

```python
{
    "businesses": [
        {...}
    ]
}
```

```go
{
    "businesses": [
        {...}
    ]
}
```

```javascript
{
    "businesses": [
        {...}
    ]
}
```

<span title="get" class="pg-type type-get">get</span>

Retrieves a business from a previously created business object.

To retrieve a business object you must supply the uniqe identifier <var>id</var> to business's resouce link
<i class="item-label">/api/v1/businesses/ <var>id</var></i> 

### HTTP Request

`GET https://dev.qebot.com/api/v1/businesses/<ID>`

### Returns
 Returns an array of a business.

## Update Business

> <b>PUT /api/v1/businesses/ <var>id</var></b>

> <b>PATCH /api/v1/businesses/ <var>id</var></b>

> Example Request

 ```shell
# Brand id needs to be appended after api uri
curl "https://dev.qebot.com/api/v1/businesses/<ID>"
  -X PATCH
  -u "<API_TOKEN>"
  -d business_name="Business Name"
  -d status=active
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
{
    "brands": [
        {...}
    ]
}
```

```php
{
    "brands": [
        {...}
    ]
}
```

```ruby
{
    "brands": [
        {...}
    ]
}
```

```python
{
    "brands": [
        {...}
    ]
}
```

```go
{
    "brands": [
        {...}
    ]
}
```

```javascript
{
    "brands": [
        {...}
    ]
}
```

<span title="put" class="pg-type type-put">post</span>
<span title="patch" class="pg-type type-patch">post</span>

Updates a business object.

To update a business object you must supply the uniqe identifier <var>id</var> to business's resouce link
<i class="item-label">/api/v1/businesses/ <var>id</var></i>

### HTTP Request

`PUT https://dev.qebot.com/api/v1/businesses/<ID>`

`PATCH https://dev.qebot.com/api/v1/businesses/<ID>`

<aside class="notice">
Even though all business params are optional.  If an empty request is passed an error will be thrown.
</aside>

<h5 class="sidebar-nav-heading">Request Arguments</h5>
Param |   | Description
----- | - | -----------
business_name | <i class="item-label">string</i><br>| Name of the business.
brand_id | <i class="item-label">integer</i> | Unique identifier for the brand of a business.  See [Brand](#brand-object) Object
category_id | <i class="item-label">integer</i> | Unique identifier for category of a business.  See [Category](#category-object) Object
phone  | <i class="item-label">string</i>| A phone contact number of the busieness.
fax  | <i class="item-label">string</i> | A fax number for the busieness.
address  | <i class="item-label">string</i>| Address of the business.
address2  | <i class="item-label">string</i> | Extra information for business address.
city  | <i class="item-label">string</i>| City of the business.
state_id  | <i class="item-label">integer</i> | Unique identifier for the state of a business. See [State](#state-object) object
state  | <i class="item-label">string</i> | Name of the state where address resides.
country_id  | <i class="item-label">integer</i>| Unique identifier for the country of a business. See [Country](#country-object) object
zipcode  | <i class="item-label">string</i>| Zipcode of the business.
email  | <i class="item-label">string</i>| Contact email for the business.
website  | <i class="item-label">string</i>| Website for the business.
status  | <i class="item-label">string</i>| Status of the business.<br />Possible values: (<b>active</b>, <b>inactive</b>)


### Returns
 Returns an array of a business.

## Delete Business

> <b>DELETE /api/v1/businesses/ <var>id</var></b>

> Example Request

 ```shell
# Brand id needs to be appended after api uri
curl "https://dev.qebot.com/api/v1/businesses/<ID>"
    -X PATCH
  -u "<API_TOKEN>"
```

 ```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

> Example Response

```shell
```

```php
 ```

```ruby
```

```python
```

```go
```

```javascript
```

<span title="delete" class="pg-type type-delete">delete</span>

Deletes a business object.

To delete a business object you must supply the uniqe identifier <var>id</var> to business's resouce link
<i class="item-label">/api/v1/businesses/ <var>id</var></i>

### HTTP Request

`DELETE https://dev.qebot.com/api/v1/businesses/<ID>`

<aside class="notice">
When a success is rendered there will be an empty response body.  You must examine status code in header to determine validity of the request.
</aside>



### Returns
 Returns an empty response.
<aside class="success">
Status code 204 is a successful response.
</aside>

<aside class="warning">
A status code of 4XX or 5XX is an unsuccesful response.
</aside>

