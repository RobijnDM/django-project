MODEL/DB FIELDS

## LISTING
id: INT
realtor: INT (FOREIGN KEY REALTOR(id_realtor))
title: CHAR VAR(150)
address: CHAR VAR(150)
city: CHAR VAR(100)
state: CHAR VAR(100)
zipcode: CHAR VAR(100)
description: TEXT
price: INT
bedrooms: INT
bathrooms: INT
sqft: INT
lot_size: FLOAT
garage: INT (DEFAULT 0)
list_date: DATE
photo_main: STR
photo_1: STR
photo_2: STR
photo_3: STR
photo_4: STR
photo_5: STR
photo_6: STR
is_published: BOOL (DEFAULT TRUE)

## REALTOR
id: INT
name: STR
photo: STR
description: STR
email: STR
phone: STR
is_mvp: BOOL (DEFAULT FALSE)
hire_date: DATE


## CONTACT
id: INT
user_id: INT 
listing: INT 
listing_id: INT
name: STR
email: STR
phone: STR
message: TEXT
contact_date: DATE