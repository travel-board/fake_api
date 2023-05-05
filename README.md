# fake_api-travel-board

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
ENDPOINTS:

# User

## Login
/USERS: POST
{
email: kenzinho@mail.com,
password: 1233456
}


## Register
/USERS: POST
{
name: user,
email: user@mail.com,
password: 1233456,
avatar: 1233456;
}

# Travels

## Recebe as travels do usuario
/TRAVELS: GET {USER BEARER TOKEN REQUIRED}
{
id: 1,
userID: 1,
name: place,
cityCountry: place,
image: placeImage,
category: beach,
}


## Adicionar travel
/TRAVELS: POST {USER BEARER TOKEN REQUIRED}
{
name: place,
cityCountry: place,
image: placeImage,
category: beach,
}

## Atualizar travel
/TRAVELS/{Travel-ID}: PATCH
{
name: place,
cityCountry: place,
image: placeImage,
category: beach,
}

## Deletar travel
/TRAVELS/{Travel-ID}: DELETE
