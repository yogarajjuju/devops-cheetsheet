# key-value pair

app: user-authentication
port: 9000
version: 1.0

# objects
microservices:
  app: user-authentication
  port: 9000
  version: 1.0

  #list
microservice:
  - app: user-authentication
    port: 9000
    version: 1.0
    #booleans -> yes , no , true , false , on and off
    deployed: true
  - app: shopping-cart
    port: 9002
    versions: [1.9,2.0, 4.0] # to represent lists in differnt way similar to arrays 


# Multiline strings  using pipe symbol |

MultilineString: |
  this is a Multiline string
  and this is next line 
  next line of other 


# to represent in a single line we use > symbol 
MultilineStr: >
  this is a Multiline string
  and this is next line 
  next line of other 


# Env variables 
# is is represented  in $ sign 

# Placeholders 
# syntax is {{}}

appp: {{ .Values.service.app}}


---


# to create seprate yaml files we need to use --- in the end 

app: user-authentication
port: 9000
version: 1.0


