Just checking out this R-package `glue` that I haven't come across
before.

    library(glue)
    library(magrittr)

    df <- mtcars

    glue('This dataset has {nrow(df)} rows and {ncol(df)} columns')

    ## This dataset has 32 rows and 11 columns

    mtcars %>% glue_data("{rownames(.)} has {cyl} cylinders and {hp} hp")

    ## Mazda RX4 has 6 cylinders and 110 hp
    ## Mazda RX4 Wag has 6 cylinders and 110 hp
    ## Datsun 710 has 4 cylinders and 93 hp
    ## Hornet 4 Drive has 6 cylinders and 110 hp
    ## Hornet Sportabout has 8 cylinders and 175 hp
    ## Valiant has 6 cylinders and 105 hp
    ## Duster 360 has 8 cylinders and 245 hp
    ## Merc 240D has 4 cylinders and 62 hp
    ## Merc 230 has 4 cylinders and 95 hp
    ## Merc 280 has 6 cylinders and 123 hp
    ## Merc 280C has 6 cylinders and 123 hp
    ## Merc 450SE has 8 cylinders and 180 hp
    ## Merc 450SL has 8 cylinders and 180 hp
    ## Merc 450SLC has 8 cylinders and 180 hp
    ## Cadillac Fleetwood has 8 cylinders and 205 hp
    ## Lincoln Continental has 8 cylinders and 215 hp
    ## Chrysler Imperial has 8 cylinders and 230 hp
    ## Fiat 128 has 4 cylinders and 66 hp
    ## Honda Civic has 4 cylinders and 52 hp
    ## Toyota Corolla has 4 cylinders and 65 hp
    ## Toyota Corona has 4 cylinders and 97 hp
    ## Dodge Challenger has 8 cylinders and 150 hp
    ## AMC Javelin has 8 cylinders and 150 hp
    ## Camaro Z28 has 8 cylinders and 245 hp
    ## Pontiac Firebird has 8 cylinders and 175 hp
    ## Fiat X1-9 has 4 cylinders and 66 hp
    ## Porsche 914-2 has 4 cylinders and 91 hp
    ## Lotus Europa has 4 cylinders and 113 hp
    ## Ford Pantera L has 8 cylinders and 264 hp
    ## Ferrari Dino has 6 cylinders and 175 hp
    ## Maserati Bora has 8 cylinders and 335 hp
    ## Volvo 142E has 4 cylinders and 109 hp
