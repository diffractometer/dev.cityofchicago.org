---
layout: post
title: New Department of Transportation permits dataset
date: '2015-11-10T18:10:32-06:00'
tags:
- avwc-kf7i
- hwmb-iu8j
- revision
- improvement
- pubx-yq2d
tumblr_url: http://chicagoportalstatus.tumblr.com/post/132963313715/new-department-of-transportation-permits-dataset
---
As part of the City of Chicago’s transition to conducting more processes paperlessly, the Department of Transportation will be implementing a new permitting system on 12/7/2015. This transition will affect datasets on the Data Portal.The following datasets will become historical only:Street Closure Permits - Current
Public Right-of-Way Use Permits
Corresponding data will be available in the new Transportation Department Permits dataset. 

We anticipate converted data back to 1/1/2013 in addition to new permit records as they are created, starting 12/7/2015.

We will update this post as more information becomes available.The current, tentative structure of the new dataset, as extracted from the https://data.cityofchicago.org/views API, is at the bottom of this post.

Update 11/10/2015 - Changed go-live date.

Update 11/16/2015 - Changed go-live date.Update 12/2/2015 - Added information on conversion data.Update 12/3/2015 - Updated tentative dataset structure.Update 12/9/2015 - The new dataset is live.Dataset structure:{  "columns": [{“id”: 232057897,“name”: “APPLICATIONNUMBER”,“dataTypeName”: “text”,“description”: “Unique number for the application that becomes the permit number when issued.”,“fieldName”: “applicationnumber”,“position”: 1,“renderTypeName”: “text”,“tableColumnId”: 29726795,“width”: 304,“format”: {“aggregate”: “count”,“align”: “left”}},{“id”: 232057898,“name”: “APPLICATIONTYPE”,“dataTypeName”: “text”,“description”: “Code for the type of permit. Permits may be categorized further by the WORKTYPE.”,“fieldName”: “applicationtype”,“position”: 2,“renderTypeName”: “text”,“tableColumnId”: 29726796,“width”: 280,“format”: {“align”: “left”}},{“id”: 232057899,“name”: “APPLICATIONDESCRIPTION”,“dataTypeName”: “text”,“description”: “Type of permit.”,“fieldName”: “applicationdescription”,“position”: 3,“renderTypeName”: “text”,“tableColumnId”: 29726797,“width”: 364,“format”: {“align”: “left”}},{“id”: 232057900,“name”: “WORKTYPE”,“dataTypeName”: “text”,“description”: “Code for the sub-category, if any, of the permit application. Only one work type per application is allowed.”,“fieldName”: “worktype”,“position”: 4,“renderTypeName”: “text”,“tableColumnId”: 29726798,“width”: 196,“format”: {“align”: “left”}},{“id”: 232057901,“name”: “WORKTYPEDESCRIPTION”,“dataTypeName”: “text”,“description”: “Sub-category, if any, of the permit application. Only one work type per application is allowed.”,“fieldName”: “worktypedescription”,“position”: 5,“renderTypeName”: “text”,“tableColumnId”: 29726799,“width”: 328,“format”: {“align”: “left”}},{“id”: 232057902,“name”: “APPLICATIONSTATUS”,“dataTypeName”: “text”,“description”: “Overall status of the application. Typically open during the application process and issued, then closed once the permit has expired.”,“fieldName”: “applicationstatus”,“position”: 6,“renderTypeName”: “text”,“tableColumnId”: 29726800,“width”: 304,“format”: {“align”: “left”}},{“id”: 232057903,“name”: “CURRENTMILESTONE”,“dataTypeName”: “text”,“description”: “The current step in the permitting life cycle.”,“fieldName”: “currentmilestone”,“position”: 7,“renderTypeName”: “text”,“tableColumnId”: 29726801,“width”: 292,“format”: {“align”: “left”}},{“id”: 232057904,“name”: “APPLICATIONSTARTDATE”,“dataTypeName”: “calendar_date”,“description”: “Permit start state. Most often requested by the applicant but could be updated as the permit is reviewed by CDOT.”,“fieldName”: “applicationstartdate”,“position”: 8,“renderTypeName”: “calendar_date”,“tableColumnId”: 29726802,“width”: 244,“format”: {“view”: “date”,“align”: “left”}},{“id”: 232057905,“name”: “APPLICATIONENDDATE”,“dataTypeName”: “calendar_date”,“description”: “Permit End state. Most often requested by the applicant but could be updated as the permit is reviewed by CDOT.”,“fieldName”: “applicationenddate”,“position”: 9,“renderTypeName”: “calendar_date”,“tableColumnId”: 29726803,“width”: 223,“format”: {“view”: “date”,“align”: “left”}},{“id”: 232057906,“name”: “APPLICATIONPROCESSEDDATE”,“dataTypeName”: “calendar_date”,“description”: “This is the date when the permit reaches the review milestone, means the date CDOT began reviewing the application.”,“fieldName”: “applicationprocesseddate”,“position”: 10,“renderTypeName”: “calendar_date”,“tableColumnId”: 29726804,“width”: 275,“format”: {“view”: “date”,“align”: “left”}},{“id”: 232057907,“name”: “APPLICATIONISSUEDDATE”,“dataTypeName”: “calendar_date”,“description”: “Date the permit was issued by CDOT. Set once all the reviews, fees, etc. are paid (where applicable).”,“fieldName”: “applicationissueddate”,“position”: 11,“renderTypeName”: “calendar_date”,“tableColumnId”: 29726805,“width”: 243,“format”: {“view”: “date”,“align”: “left”}},{“id”: 232057908,“name”: “APPLICATIONFINALIZEDDATE”,“dataTypeName”: “calendar_date”,“description”: “Date the permit was closed (either after the permit has expired plus a grace period or after an inspector marks the work complete).”,“fieldName”: “applicationfinalizeddate”,“position”: 12,“renderTypeName”: “calendar_date”,“tableColumnId”: 29726806,“width”: 266,“format”: {“view”: “date”,“align”: “left”}},{“id”: 232057909,“name”: “APPLICATIONEXPIREDATE”,“dataTypeName”: “calendar_date”,“description”: “Date the permit will expire (typically same as permit end date). Applicant may ask for date extensions where the end date is updated and will be reflected here once re-approved by CDOT.”,“fieldName”: “applicationexpiredate”,“position”: 13,“renderTypeName”: “calendar_date”,“tableColumnId”: 29726807,“width”: 245,“format”: {“view”: “date”,“align”: “left”}},{“id”: 232057911,“name”: “APPLICATIONNAME”,“dataTypeName”: “text”,“description”: “Applicants can put a project name on their applications in this field. For converted data 1/1/2013 to 11/13/2015, the old permit number will be placed in this field.”,“fieldName”: “applicationname”,“position”: 14,“renderTypeName”: “text”,“tableColumnId”: 29726808,“width”: 280,“format”: {“align”: “left”}},{“id”: 232057912,“name”: “COMMENTS”,“dataTypeName”: “text”,“description”: “Applicants can place a description of the work here.”,“fieldName”: “comments”,“position”: 15,“renderTypeName”: “text”,“tableColumnId”: 29726809,“width”: 196,“format”: {“align”: “left”}},{“id”: 232057913,“name”: “TOTALFEES”,“dataTypeName”: “money”,“description”: “Total permit fees for this permit calculated based on the work being carried out and location. See fee schedule for further information, available on the CDOT permit portal, http://www.cityofchicago.org/city/en/depts/cdot/provdrs/construction_information/svcs/online-permit-portal.html.”,“fieldName”: “totalfees”,“position”: 16,“renderTypeName”: “money”,“tableColumnId”: 29726810,“width”: 208,“format”: {“aggregate”: “sum”,“humane”: “false”,“currency”: “USD”,“align”: “right”}},{“id”: 232057914,“name”: “WAIVEDFEES”,“dataTypeName”: “money”,“description”: “If any fees were waived for this permit, the amount waived will be here. Possible reasons for waived fees include city contracts, city departments, ordinances, and franchise agreements with the City. ”,“fieldName”: “waivedfees”,“position”: 17,“renderTypeName”: “money”,“tableColumnId”: 29726811,“width”: 220,“format”: {“precisionStyle”: “standard”,“noCommas”: “false”,“align”: “right”}},{“id”: 232057915,“name”: “PRIMARYCONTACTLAST”,“dataTypeName”: “text”,“description”: “The last name of the primary applicant for the permit. If an employee applied on behalf of a company, the company name will appear. ”,“fieldName”: “primarycontactlast”,“position”: 18,“renderTypeName”: “text”,“tableColumnId”: 29726812,“width”: 316,“format”: {“align”: “left”}},{“id”: 232057916,“name”: “PRIMARYCONTACTFIRST”,“dataTypeName”: “text”,“description”: “First name of the primary applicant, if not a company.”,“fieldName”: “primarycontactfirst”,“position”: 19,“renderTypeName”: “text”,“tableColumnId”: 29726813,“width”: 240,“format”: {“align”: “left”}},{“id”: 232057917,“name”: “PRIMARYCONTACTMIDDLE”,“dataTypeName”: “text”,“description”: “Middle initial of the primary applicant, if not a company.”,“fieldName”: “primarycontactmiddle”,“position”: 20,“renderTypeName”: “text”,“tableColumnId”: 29726814,“width”: 255,“format”: {“align”: “left”}},{“id”: 232057918,“name”: “PRIMARYCONTACTSTREET”,“dataTypeName”: “text”,“description”: “Street address of the primary applicant.”,“fieldName”: “primarycontactstreet”,“position”: 21,“renderTypeName”: “text”,“tableColumnId”: 29726815,“width”: 261,“format”: {“align”: “left”}},{“id”: 232057919,“name”: “PRIMARYCONTACTSTREET2”,“dataTypeName”: “text”,“description”: “Street address 2nd line of the primary applicant.”,“fieldName”: “primarycontactstreet2”,“position”: 22,“renderTypeName”: “text”,“tableColumnId”: 29726816,“width”: 257,“format”: {“align”: “left”}},{“id”: 232057920,“name”: “PRIMARYCONTACTCITY”,“dataTypeName”: “text”,“description”: “City of the primary applicant.”,“fieldName”: “primarycontactcity”,“position”: 23,“renderTypeName”: “text”,“tableColumnId”: 29726817,“width”: 251,“format”: {“align”: “left”}},{“id”: 232057921,“name”: “PRIMARYCONTACTSTATE”,“dataTypeName”: “text”,“description”: “State of the primary applicant.”,“fieldName”: “primarycontactstate”,“position”: 24,“renderTypeName”: “text”,“tableColumnId”: 29726818,“width”: 249,“format”: {“align”: “left”}},{“id”: 232057922,“name”: “PRIMARYCONTACTZIP”,“dataTypeName”: “text”,“description”: “ZIP Code of the primary applicant.”,“fieldName”: “primarycontactzip”,“position”: 25,“renderTypeName”: “text”,“tableColumnId”: 29726819,“width”: 223,“format”: {“align”: “left”}},{“id”: 232057925,“name”: “EMERGENCYCONTACTNAME”,“dataTypeName”: “text”,“description”: “Person to contact in an emergency as listed by the applicant during the permit application process.”,“fieldName”: “emergencycontactname”,“position”: 28,“renderTypeName”: “text”,“tableColumnId”: 29726822,“width”: 273,“format”: {“align”: “left”}},{“id”: 232057929,“name”: “LASTINSPECTIONNUMBER”,“dataTypeName”: “number”,“description”: “Once a permit is issued, typically an inspection is created for CDOT Inspectors to use onsite. Once an inspection is completed, another inspection may be generated or if the work is finished, the permit is closed. This is the number of the last inspection.”,“fieldName”: “lastinspectionnumber”,“position”: 32,“renderTypeName”: “number”,“tableColumnId”: 29726826,“width”: 251,“format”: {“precisionStyle”: “standard”,“align”: “right”,“noCommas”: “true”}},{“id”: 232057930,“name”: “LASTINSPECTIONTYPE”,“dataTypeName”: “text”,“description”: “Code for the type of inspection generated for the issued permit. Typically this will match the type of permit although special inspection types are available for stop work.”,“fieldName”: “lastinspectiontype”,“position”: 33,“renderTypeName”: “text”,“tableColumnId”: 29726827,“width”: 223,“format”: {“align”: “left”}},{“id”: 232057931,“name”: “LASTINSPTYPEDESCR”,“dataTypeName”: “text”,“description”: “Description of the last inspection completed against this permit.”,“fieldName”: “lastinsptypedescr”,“position”: 34,“renderTypeName”: “text”,“tableColumnId”: 29726828,“width”: 304,“format”: {“align”: “left”}},{“id”: 232057932,“name”: “LASTINSPECTIONDATE”,“dataTypeName”: “calendar_date”,“description”: “Date of the last inspection.”,“fieldName”: “lastinspectiondate”,“position”: 35,“renderTypeName”: “calendar_date”,“tableColumnId”: 29726829,“width”: 229,“format”: {“view”: “date”,“align”: “left”}},{“id”: 232057933,“name”: “LASTINSPECTIONRESULT”,“dataTypeName”: “text”,“description”: “The result of the last inspection, if completed.”,“fieldName”: “lastinspectionresult”,“position”: 36,“renderTypeName”: “text”,“tableColumnId”: 29726830,“width”: 239,“format”: {“align”: “left”}},{“id”: 232057935,“name”: “STREETNUMBERFROM”,“dataTypeName”: “number”,“description”: “The start of the address range for the permit location. For multiple locations on a permit, there will be multiple rows in the dataset.”,“fieldName”: “streetnumberfrom”,“position”: 38,“renderTypeName”: “number”,“tableColumnId”: 29726832,“width”: 225,“format”: {“precisionStyle”: “standard”,“align”: “right”,“noCommas”: “true”}},{“id”: 232057936,“name”: “STREETNUMBERTO”,“dataTypeName”: “number”,“description”: “The end of the address range for the permit location. For multiple locations on a permit, there will be multiple rows in the dataset.”,“fieldName”: “streetnumberto”,“position”: 39,“renderTypeName”: “number”,“tableColumnId”: 29726833,“width”: 210,“format”: {“precisionStyle”: “standard”,“align”: “right”,“noCommas”: “true”}},{“id”: 232057937,“name”: “DIRECTION”,“dataTypeName”: “text”,“description”: “The street direction for the permit location. For multiple locations on a permit, there will be multiple rows in the dataset.”,“fieldName”: “direction”,“position”: 40,“renderTypeName”: “text”,“tableColumnId”: 29726834,“width”: 154,“format”: {“align”: “left”}},{“id”: 232057938,“name”: “STREETNAME”,“dataTypeName”: “text”,“description”: “The street name for the permit location. For multiple locations on a permit, there will be multiple rows in the dataset.”,“fieldName”: “streetname”,“position”: 41,“renderTypeName”: “text”,“tableColumnId”: 29726835,“width”: 220,“format”: {“align”: “left”}},{“id”: 232057939,“name”: “SUFFIX”,“dataTypeName”: “text”,“description”: “The street name suffix for the permit location. For multiple locations on a permit, there will be multiple rows in the dataset.”,“fieldName”: “suffix”,“position”: 42,“renderTypeName”: “text”,“tableColumnId”: 29726836,“width”: 130,“format”: {“align”: “left”}},{“id”: 232057940,“name”: “PLACEMENT”,“dataTypeName”: “text”,“description”: “Additional information about the permit location. This column may also include detour information.”,“fieldName”: “placement”,“position”: 43,“renderTypeName”: “text”,“tableColumnId”: 29726837,“width”: 166,“format”: {“align”: “left”}},{“id”: 232057941,“name”: “STREETCLOSURE”,“dataTypeName”: “text”,“description”: “Type of street closure, if any, associated with the location.”,“fieldName”: “streetclosure”,“position”: 44,“renderTypeName”: “text”,“tableColumnId”: 29726838,“width”: 193,“format”: {“align”: “left”}},{“id”: 232057942,“name”: “DETAIL”,“dataTypeName”: “text”,“description”: “Detail information about the permit application.”,“fieldName”: “detail”,“position”: 45,“renderTypeName”: “text”,“tableColumnId”: 32446183,“width”: 321,“format”: {“align”: “left”}},{“id”: 232057943,“name”: “PARKINGMETERPOSTINGORBAGGING”,“dataTypeName”: “text”,“description”: “Indicates if any parking meter bagging or posting of no parking signs  is requested on the permit application.”,“fieldName”: “parkingmeterpostingorbagging”,“position”: 46,“renderTypeName”: “text”,“tableColumnId”: 29726839,“width”: 317,“format”: {“align”: “left”}},{“id”: 232057944,“name”: “LATITUDE”,“dataTypeName”: “number”,“description”: “Latitude of the start of the address range.”,“fieldName”: “latitude”,“position”: 47,“renderTypeName”: “number”,“tableColumnId”: 29726840,“width”: 153,“format”: {“precisionStyle”: “standard”,“align”: “right”,“noCommas”: “false”}},{“id”: 232057945,“name”: “LONGITUDE”,“dataTypeName”: “number”,“description”: “Longitude of the start of the address range.”,“fieldName”: “longitude”,“position”: 48,“renderTypeName”: “number”,“tableColumnId”: 29726841,“width”: 164,“format”: {“precisionStyle”: “standard”,“align”: “right”,“noCommas”: “false”}},{“id”: 232057946,“name”: “LOCATION”,“dataTypeName”: “location”,“description”: “Location of the start of the address range.”,“fieldName”: “location”,“position”: 49,“renderTypeName”: “location”,“tableColumnId”: 29726842,“width”: 196,“format”: {“view”: “coords”,“align”: “left”},“subColumnTypes”: [“human_address”,“latitude”,“longitude”,“machine_address”,“needs_recoding”]}]  }