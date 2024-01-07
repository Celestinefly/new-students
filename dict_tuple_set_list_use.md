## Summarize the usage of dictionaries, tuples, sets, and lists in Python  

-----

### 1.the usage of dictionary  
  
```python
#create
person1={'name':'linlin','age':18,'gender':'female'}
person2=dict(name='feifei',age='19',gender='male')xxxxxxS
print(person1['name'])
print(person2['name'])
```
```python
#add
person1={'name':'linlin','age':18,'gender':'female'}
person2=dict(name='feifei',age='19',gender='male')
person1['birthday']='2006-1-27'
person2['birthday']='2005-8-24'
print('new two persons')
print(person1)
print(person2)
```
```pythone
#delete 
person1={'name':'linlin','age':18,'gender':'female'}
person2=dict(name='feifei',age='19',gender='male')
del person1['name']
del person2['age']
print('new two persons')
print(person1)
print(person2)
```
```python
#change
person1={'name':'linlin','age':18,'gender':'female'}
person2=dict(name='feifei',age='19',gender='male')
person2["name"]="xiaohu"
print(person2)
```
```python
#search for
person1={'name':'linlin','age':18,'gender':'female'}
person2=dict(name='feifei',age='19',gender='male')
print(person1.keys())
print(person2.values())
print(person1.items())
```
----
### 2.the usage of tuple
```python
#create
tuple=(1,2,3,4,5)


   

