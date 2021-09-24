# dataset_part1	

	
This directory shows database schemas and class diagrams extracted via java programs (from JPA and/or Hibernate programs). In each directory you will find these files:

```txt
-1- The class diagram which includes all the java classes that are in this project (They can be used and visualized by EMF(Eclipse Modeling Framework))
    --> allClasses.ecore
    --> allClasses.xsd 
    
-2- The class diagram which includes all entities(Domain Model or the layer of DAO (Data Access Objects)) that are in this project.
    --> DomainModel.ecore
    --> DomainModel.xsd 
    
-3- We can find several SRC directories in a single Github project (this is why we see that the name of the generated directories () is greater than the number of repo (2184 Github directory)), in the file Git_Link.txt you can find the link to SRC directory on Github.
    --> Git_Link.txt
    
-4- The relational schema implemented in the RDBMS used by this program.  
--> RelationelSchema_Inheritance.txt

-5- The mapping between the domain model (2) and the relational schema (4)
--> Mapping.txt
```    
Repo: 2183; Output directories: 3739;
# Links
List of project : https://github.com/KhalidBelharbi/JPA-Hibernate-projects-on-Github

Part1: https://github.com/KhalidBelharbi/Geodes_dataset_part1/tree/master

Part2: https://github.com/KhalidBelharbi/Geodes_dataset_part2/tree/master

Part3: https://github.com/KhalidBelharbi/Geodes_dataset_part3/tree/master

# Exemple of Output
we can show the result obtained for the program which is below the link: [2019_San-giao-dich-trang-tri-noi-that](https://github.com/anhtuangithub/2019_San-giao-dich-trang-tri-noi-that/tree/master/luanvan/src)

## Git_Link.txt
```txt
Local Path: /u/belharbk/dataset/2019_San-giao-dich-trang-tri-noi-that/luanvan/src
Github Link:https://github.com/anhtuangithub/2019_San-giao-dich-trang-tri-noi-that/tree/master/luanvan/src
```
## RelationelSchema_Inheritance.txt
```txt

orderstatus(id:Long [PK], name:String, status:int);

color(id:Long [PK], name:String, status:int);

product(id:Long [PK], name:String, plug:String, description:String, quantity:int, avatar:String, avgstart:float, created_at:Date, upd_at:Date, status:int, s:Category #FK to(Category), s:Store #FK to(Store), s:Producer #FK to(Producer), s:Origin #FK to(origin), s:Material #FK to(Material));

product_color(product_id:Product [PK] #FK to Product,color_id:Color [PK] #FK to Color);

image360(id:Long [PK], path:String, status:int, _id:Product #FK to(Product));

province(provinceid:String [PK], name:String);

district(districtid:String [PK], name:String, provinceid:String);

review(id:Long [PK], content:String, rating:int, status:int, created_at:Date, upd_at:Date, user:Users #FK to(Users), s:Product #FK to(Product), GeneratedName:Order #FK to(Order));

image(id:Long [PK], path:String, status:int, _id:Product #FK to(Product));

paymenttype(id:Long [PK], name:String, status:int);

passwordresettoken(id:Long [PK], token:String, user:Users #FK to(Users), expiry:Date);

unitprice(id:Long [PK], price:int, created_at:Date, start_time:Date, end_time:Date, root:int, GeneratedName:Product #FK to(Product));

answer(id:Long [PK], content:String, status:int, created_at:Date, s:Question #FK to(Question), s:Store #FK to(Store));

customer(id:Long [PK], name:String, address:String, sex:String, phone:String, birthday:Date, GeneratedName:Users #FK to(Users));

store(id:Long [PK], name:String, address:String, phone:String, introduce:String, website:String, status:int, GeneratedName:Users #FK to(Users), GeneratedName:Province #FK to(Province), GeneratedName:District #FK to(District), GeneratedName:Ward #FK to(Ward));

member(id:Long [PK], start_time:Date, end_time:Date, s:MemberType #FK to(Member), s:Store #FK to(Store));

question(id:Long [PK], content:String, status:int, created_at:Date, s:Product #FK to(Product), user:Users #FK to(Users));

membertype(id:Long [PK], name:String, price:int);

role(id:Long [PK], name:String);

inventory(id:Long [PK], quantity:int, created_at:Date, _receipt:Date, s:Product #FK to(Product));

promotion(id:Long [PK], name:String, description:String, sale_off:int, status:int, created_at:Date, start_time:Date, end_time:Date, GeneratedName:Store #FK to(Store));

product_promotion(promotion_id:Promotion [PK] #FK to Promotion,product_id:Product [PK] #FK to Product);

ward(wardid:String [PK], name:String, districtid:String);

orderdetail(id:OrderDetailId, quantity:int, GeneratedName:Product #FK to(Product), s:Order #FK to(Order), s:Color #FK to(Color), GeneratedName:UnitPrice #FK to(UnitPrice), GeneratedName:Promotion #FK to(Promotion));

users(id:Long [PK], email:String, password:String, GeneratedName:Store #FK to(Store), GeneratedName:Customer #FK to(Customer));

user_role(user_id:Users [PK] #FK to Users,role_id:Role [PK] #FK to Role);

producer(id:Long [PK], name:String, status:int, plug:String);

order(id:Long [PK], address:String, phone:String, created_at:Date, GeneratedName:PaymentType #FK to(PaymentType), user:Users #FK to(Users), GeneratedName:OrderStatus #FK to(OrderStatus), GeneratedName:OrderGroup #FK to(Order), s:Store #FK to(Store));

category(id:Long [PK], name:String, plug:String, parentid:Long, status:int);

material(id:Long [PK], name:String, plug:String, status:int);

origin(id:Long [PK], name:String, plug:String, status:int);

ordergroup(id:Long [PK], address:String, phone:String, created_at:Date, GeneratedName:PaymentType #FK to(PaymentType), user:Users #FK to(Users));

** PROGRAM TYPE: JPA+Hibernate(Hybrid)
```
## DomainModel.ecore

<img src="Exemple of generated EMF file.png"></img>
<img src="Exemple of results-DomainModel class diagram(EMF).jpg"></img>

```xml
<?xml version="1.0" encoding="UTF-8"?>
<ecore:EPackage xmi:version="2.0" xmlns:xmi="http://www.omg.org/XMI" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:ecore="http://www.eclipse.org/emf/2002/Ecore" name="DomainModel" nsURI="file:/part/01/Tmp/belharbk/2019_San-giao-dich-trang-tri-noi-that/DomainModel.xsd"
    nsPrefix="DomainModel">
  <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
    <details key="qualified" value="false"/>
  </eAnnotations>
  <eClassifiers xsi:type="ecore:EClass" name="Answer">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="answer"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="content" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="content"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s" eType="#//Question"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s1" eType="#//Store" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Category">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="category"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="plug" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="plug"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="parentid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="parentid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="product" upperBound="-1"
        eType="#//Product" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="product"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Color">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="color"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orderdetails" upperBound="-1"
        eType="#//Orderdetail" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orderdetails"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="products" upperBound="-1"
        eType="#//Product" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="products"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Customer">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="customer"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="address" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="address"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="sex" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="sex"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="phone" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="phone"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="birthday" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="birthday"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Users"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="District">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="district"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="districtid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="districtid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="provinceid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="provinceid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="stores" upperBound="-1"
        eType="#//Store" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="stores"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Image">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="image"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="path" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="path"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="id1" eType="#//Product"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="_id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Image360">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="image360"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="path" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="path"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="id1" eType="#//Product"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="_id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Inventory">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="inventory"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="quantity" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="quantity"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="receipt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="_receipt"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s" eType="#//Product" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Material">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="material"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="plug" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="plug"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="products" upperBound="-1"
        eType="#//Product" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="products"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Member">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="member"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="startTime" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="start_time"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="endTime" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="end_time"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s" eType="#//Membertype"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s1" eType="#//Store" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Membertype">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="membertype"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="price" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="price"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="members" upperBound="-1"
        eType="#//Member" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="members"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Order">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="order"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="address" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="address"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="phone" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="phone"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orderdetail" upperBound="-1"
        eType="#//Orderdetail" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orderdetail"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="review" upperBound="-1"
        eType="#//Review" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="review"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Paymenttype"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="user" eType="#//Users"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="user"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName1" eType="#//Orderstatus"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName2" eType="#//Ordergroup"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s" eType="#//Store" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Orderdetail">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="orderdetail"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//AnySimpleType"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="quantity" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="quantity"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Product"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s" eType="#//Order" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s1" eType="#//Color" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName1" eType="#//Unitprice"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName2" eType="#//Promotion"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Ordergroup">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="ordergroup"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="address" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="address"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="phone" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="phone"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orders" upperBound="-1"
        eType="#//Order" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orders"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Paymenttype"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="user" eType="#//Users"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="user"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Orderstatus">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="orderstatus"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orders" upperBound="-1"
        eType="#//Order" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orders"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Origin">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="origin"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="plug" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="plug"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="products" upperBound="-1"
        eType="#//Product" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="products"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Passwordresettoken">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="passwordresettoken"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="token" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="token"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="user" eType="#//Users"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="user"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="expiry" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="expiry"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Paymenttype">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="paymenttype"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orders" upperBound="-1"
        eType="#//Order" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orders"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="ordergroup" upperBound="-1"
        eType="#//Ordergroup" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="ordergroup"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Producer">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="producer"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="plug" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="plug"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="products" upperBound="-1"
        eType="#//Product" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="products"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Product">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="product"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="plug" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="plug"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="description" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="description"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="quantity" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="quantity"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="avatar" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="avatar"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="avgstart" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Double" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="avgstart"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="updAt" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="upd_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="inventory" upperBound="-1"
        eType="#//Inventory" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="inventory"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="questions" upperBound="-1"
        eType="#//Question" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="questions"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="images" upperBound="-1"
        eType="#//Image" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="images"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="image360" upperBound="-1"
        eType="#//Image360" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="image360"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orderdetails" upperBound="-1"
        eType="#//Orderdetail" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orderdetails"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="reviews" upperBound="-1"
        eType="#//Review" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="reviews"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="unitprices" upperBound="-1"
        eType="#//Unitprice" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="unitprices"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orderdetail" upperBound="-1"
        eType="#//Orderdetail" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orderdetail"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s" eType="#//Category"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s1" eType="#//Store" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s2" eType="#//Producer"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s3" eType="#//Origin" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s4" eType="#//Material"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="colors" upperBound="-1"
        eType="#//Color" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="colors"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="promotions" upperBound="-1"
        eType="#//Promotion" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="promotions"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Promotion">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="promotion"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="description" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="description"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="saleOff" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="sale_off"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="startTime" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="start_time"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="endTime" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="end_time"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orderdetail" upperBound="-1"
        eType="#//Orderdetail" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orderdetail"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Store"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="products" upperBound="-1"
        eType="#//Product" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="products"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Province">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="province"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="provinceid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="provinceid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="stores" upperBound="-1"
        eType="#//Store" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="stores"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Question">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="question"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="content" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="content"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="answers" upperBound="-1"
        eType="#//Answer" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="answers"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s" eType="#//Product" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="user" eType="#//Users"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="user"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Review">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="review"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="content" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="content"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="rating" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="rating"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="updAt" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="upd_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="user" eType="#//Users"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="user"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="s" eType="#//Product" unsettable="true"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="s"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Order"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Role">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="role"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="users" upperBound="-1"
        eType="#//Users" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="users"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Store">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="store"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="address" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="address"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="phone" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="phone"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="introduce" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="introduce"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="website" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="website"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="status" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="status"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Users"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="answers" upperBound="-1"
        eType="#//Answer" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="answers"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orders" upperBound="-1"
        eType="#//Order" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orders"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="products" upperBound="-1"
        eType="#//Product" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="products"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="promotions" upperBound="-1"
        eType="#//Promotion" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="promotions"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="members" upperBound="-1"
        eType="#//Member" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="members"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName1" eType="#//Province"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName2" eType="#//District"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName3" eType="#//Ward"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Unitprice">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="unitprice"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="price" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="price"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="createdAt" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="created_at"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="startTime" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="start_time"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="endTime" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="end_time"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="root" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="root"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="orderdetails" upperBound="-1"
        eType="#//Orderdetail" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orderdetails"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Product"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Users">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="users"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="id" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long"
        unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="id"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="email" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="email"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="password" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="password"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName" eType="#//Store"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="generatedName1" eType="#//Customer"
        unsettable="true" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="GeneratedName"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="order" upperBound="-1"
        eType="#//Order" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="order"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="ordergroup" upperBound="-1"
        eType="#//Ordergroup" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="ordergroup"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="reviews" upperBound="-1"
        eType="#//Review" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="reviews"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="questions" upperBound="-1"
        eType="#//Question" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="questions"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="roles" upperBound="-1"
        eType="#//Role" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="roles"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Ward">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="ward"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="wardid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="wardid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="name" lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="name"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="districtid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="districtid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EReference" name="stores" upperBound="-1"
        eType="#//Store" containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="stores"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
</ecore:EPackage>
```
## Mapping.txt
```txt
ClassDiagram.Class>> OrderStatus =>=>=> RelationalSchema.Table>> orderstatus;
ClassDiagram.Class>> Color =>=>=> RelationalSchema.Table>> color;
ClassDiagram.Class>> Product =>=>=> RelationalSchema.Table>> product;
ClassDiagram.Class>> Image360 =>=>=> RelationalSchema.Table>> image360;
ClassDiagram.Class>> Province =>=>=> RelationalSchema.Table>> province;
ClassDiagram.Class>> District =>=>=> RelationalSchema.Table>> district;
ClassDiagram.Class>> Review =>=>=> RelationalSchema.Table>> review;
ClassDiagram.Class>> Image =>=>=> RelationalSchema.Table>> image;
ClassDiagram.Class>> PaymentType =>=>=> RelationalSchema.Table>> paymenttype;
ClassDiagram.Class>> PasswordResetToken =>=>=> RelationalSchema.Table>> passwordresettoken;
ClassDiagram.Class>> UnitPrice =>=>=> RelationalSchema.Table>> unitprice;
ClassDiagram.Class>> Answer =>=>=> RelationalSchema.Table>> answer;
ClassDiagram.Class>> Customer =>=>=> RelationalSchema.Table>> customer;
ClassDiagram.Class>> Store =>=>=> RelationalSchema.Table>> store;
ClassDiagram.Class>> Member =>=>=> RelationalSchema.Table>> member;
ClassDiagram.Class>> Question =>=>=> RelationalSchema.Table>> question;
ClassDiagram.Class>> MemberType =>=>=> RelationalSchema.Table>> membertype;
ClassDiagram.Class>> Role =>=>=> RelationalSchema.Table>> role;
ClassDiagram.Class>> Inventory =>=>=> RelationalSchema.Table>> inventory;
ClassDiagram.Class>> Promotion =>=>=> RelationalSchema.Table>> promotion;
ClassDiagram.Class>> Ward =>=>=> RelationalSchema.Table>> ward;
ClassDiagram.Class>> OrderDetail =>=>=> RelationalSchema.Table>> orderdetail;
ClassDiagram.Class>> Users =>=>=> RelationalSchema.Table>> users;
ClassDiagram.Class>> Producer =>=>=> RelationalSchema.Table>> producer;
ClassDiagram.Class>> Order =>=>=> RelationalSchema.Table>> order;
ClassDiagram.Class>> Category =>=>=> RelationalSchema.Table>> category;
ClassDiagram.Class>> Material =>=>=> RelationalSchema.Table>> material;
ClassDiagram.Class>> Origin =>=>=> RelationalSchema.Table>> origin;
ClassDiagram.Class>> OrderGroup =>=>=> RelationalSchema.Table>> ordergroup;
ClassDiagram.Attribut>> OrderStatus.id:Long =>=>=> RelationalSchema.Column>> orderstatus.id PRIMARY KEY;
ClassDiagram.Attribut>> OrderStatus.name:String =>=>=> RelationalSchema.Column>> orderstatus.name;
ClassDiagram.Attribut>> OrderStatus.status:int =>=>=> RelationalSchema.Column>> orderstatus.status;
ClassDiagram.Attribut>> Color.id:Long =>=>=> RelationalSchema.Column>> color.id PRIMARY KEY;
ClassDiagram.Attribut>> Color.name:String =>=>=> RelationalSchema.Column>> color.name;
ClassDiagram.Attribut>> Color.status:int =>=>=> RelationalSchema.Column>> color.status;
ClassDiagram.Attribut>> Product.id:Long =>=>=> RelationalSchema.Column>> product.id PRIMARY KEY;
ClassDiagram.Attribut>> Product.name:String =>=>=> RelationalSchema.Column>> product.name;
ClassDiagram.Attribut>> Product.plug:String =>=>=> RelationalSchema.Column>> product.plug;
ClassDiagram.Attribut>> Product.description:String =>=>=> RelationalSchema.Column>> product.description;
ClassDiagram.Attribut>> Product.quantity:int =>=>=> RelationalSchema.Column>> product.quantity;
ClassDiagram.Attribut>> Product.avatar:String =>=>=> RelationalSchema.Column>> product.avatar;
ClassDiagram.Attribut>> Product.avgstart:float =>=>=> RelationalSchema.Column>> product.avgstart;
ClassDiagram.Attribut>> Product.created_at:Date =>=>=> RelationalSchema.Column>> product.created_at;
ClassDiagram.Attribut>> Product.upd_at:Date =>=>=> RelationalSchema.Column>> product.upd_at;
ClassDiagram.Attribut>> Product.status:int =>=>=> RelationalSchema.Column>> product.status;
ClassDiagram.Attribut>> Image360.id:Long =>=>=> RelationalSchema.Column>> image360.id PRIMARY KEY;
ClassDiagram.Attribut>> Image360.path:String =>=>=> RelationalSchema.Column>> image360.path;
ClassDiagram.Attribut>> Image360.status:int =>=>=> RelationalSchema.Column>> image360.status;
ClassDiagram.Attribut>> Province.provinceid:String =>=>=> RelationalSchema.Column>> province.provinceid PRIMARY KEY;
ClassDiagram.Attribut>> Province.name:String =>=>=> RelationalSchema.Column>> province.name;
ClassDiagram.Attribut>> District.districtid:String =>=>=> RelationalSchema.Column>> district.districtid PRIMARY KEY;
ClassDiagram.Attribut>> District.name:String =>=>=> RelationalSchema.Column>> district.name;
ClassDiagram.Attribut>> District.provinceid:String =>=>=> RelationalSchema.Column>> district.provinceid;
ClassDiagram.Attribut>> Review.id:Long =>=>=> RelationalSchema.Column>> review.id PRIMARY KEY;
ClassDiagram.Attribut>> Review.content:String =>=>=> RelationalSchema.Column>> review.content;
ClassDiagram.Attribut>> Review.rating:int =>=>=> RelationalSchema.Column>> review.rating;
ClassDiagram.Attribut>> Review.status:int =>=>=> RelationalSchema.Column>> review.status;
ClassDiagram.Attribut>> Review.created_at:Date =>=>=> RelationalSchema.Column>> review.created_at;
ClassDiagram.Attribut>> Review.upd_at:Date =>=>=> RelationalSchema.Column>> review.upd_at;
ClassDiagram.Attribut>> Image.id:Long =>=>=> RelationalSchema.Column>> image.id PRIMARY KEY;
ClassDiagram.Attribut>> Image.path:String =>=>=> RelationalSchema.Column>> image.path;
ClassDiagram.Attribut>> Image.status:int =>=>=> RelationalSchema.Column>> image.status;
ClassDiagram.Attribut>> PaymentType.id:Long =>=>=> RelationalSchema.Column>> paymenttype.id PRIMARY KEY;
ClassDiagram.Attribut>> PaymentType.name:String =>=>=> RelationalSchema.Column>> paymenttype.name;
ClassDiagram.Attribut>> PaymentType.status:int =>=>=> RelationalSchema.Column>> paymenttype.status;
ClassDiagram.Attribut>> PasswordResetToken.id:Long =>=>=> RelationalSchema.Column>> passwordresettoken.id PRIMARY KEY;
ClassDiagram.Attribut>> PasswordResetToken.token:String =>=>=> RelationalSchema.Column>> passwordresettoken.token;
ClassDiagram.Attribut>> PasswordResetToken.expiry:Date =>=>=> RelationalSchema.Column>> passwordresettoken.expiry;
ClassDiagram.Attribut>> UnitPrice.id:Long =>=>=> RelationalSchema.Column>> unitprice.id PRIMARY KEY;
ClassDiagram.Attribut>> UnitPrice.price:int =>=>=> RelationalSchema.Column>> unitprice.price;
ClassDiagram.Attribut>> UnitPrice.created_at:Date =>=>=> RelationalSchema.Column>> unitprice.created_at;
ClassDiagram.Attribut>> UnitPrice.start_time:Date =>=>=> RelationalSchema.Column>> unitprice.start_time;
ClassDiagram.Attribut>> UnitPrice.end_time:Date =>=>=> RelationalSchema.Column>> unitprice.end_time;
ClassDiagram.Attribut>> UnitPrice.root:int =>=>=> RelationalSchema.Column>> unitprice.root;
ClassDiagram.Attribut>> Answer.id:Long =>=>=> RelationalSchema.Column>> answer.id PRIMARY KEY;
ClassDiagram.Attribut>> Answer.content:String =>=>=> RelationalSchema.Column>> answer.content;
ClassDiagram.Attribut>> Answer.status:int =>=>=> RelationalSchema.Column>> answer.status;
ClassDiagram.Attribut>> Answer.created_at:Date =>=>=> RelationalSchema.Column>> answer.created_at;
ClassDiagram.Attribut>> Customer.id:Long =>=>=> RelationalSchema.Column>> customer.id PRIMARY KEY;
ClassDiagram.Attribut>> Customer.name:String =>=>=> RelationalSchema.Column>> customer.name;
ClassDiagram.Attribut>> Customer.address:String =>=>=> RelationalSchema.Column>> customer.address;
ClassDiagram.Attribut>> Customer.sex:String =>=>=> RelationalSchema.Column>> customer.sex;
ClassDiagram.Attribut>> Customer.phone:String =>=>=> RelationalSchema.Column>> customer.phone;
ClassDiagram.Attribut>> Customer.birthday:Date =>=>=> RelationalSchema.Column>> customer.birthday;
ClassDiagram.Attribut>> Store.id:Long =>=>=> RelationalSchema.Column>> store.id PRIMARY KEY;
ClassDiagram.Attribut>> Store.name:String =>=>=> RelationalSchema.Column>> store.name;
ClassDiagram.Attribut>> Store.address:String =>=>=> RelationalSchema.Column>> store.address;
ClassDiagram.Attribut>> Store.phone:String =>=>=> RelationalSchema.Column>> store.phone;
ClassDiagram.Attribut>> Store.introduce:String =>=>=> RelationalSchema.Column>> store.introduce;
ClassDiagram.Attribut>> Store.website:String =>=>=> RelationalSchema.Column>> store.website;
ClassDiagram.Attribut>> Store.status:int =>=>=> RelationalSchema.Column>> store.status;
ClassDiagram.Attribut>> Member.id:Long =>=>=> RelationalSchema.Column>> member.id PRIMARY KEY;
ClassDiagram.Attribut>> Member.start_time:Date =>=>=> RelationalSchema.Column>> member.start_time;
ClassDiagram.Attribut>> Member.end_time:Date =>=>=> RelationalSchema.Column>> member.end_time;
ClassDiagram.Attribut>> Question.id:Long =>=>=> RelationalSchema.Column>> question.id PRIMARY KEY;
ClassDiagram.Attribut>> Question.content:String =>=>=> RelationalSchema.Column>> question.content;
ClassDiagram.Attribut>> Question.status:int =>=>=> RelationalSchema.Column>> question.status;
ClassDiagram.Attribut>> Question.created_at:Date =>=>=> RelationalSchema.Column>> question.created_at;
ClassDiagram.Attribut>> MemberType.id:Long =>=>=> RelationalSchema.Column>> membertype.id PRIMARY KEY;
ClassDiagram.Attribut>> MemberType.name:String =>=>=> RelationalSchema.Column>> membertype.name;
ClassDiagram.Attribut>> MemberType.price:int =>=>=> RelationalSchema.Column>> membertype.price;
ClassDiagram.Attribut>> Role.id:Long =>=>=> RelationalSchema.Column>> role.id PRIMARY KEY;
ClassDiagram.Attribut>> Role.name:String =>=>=> RelationalSchema.Column>> role.name;
ClassDiagram.Attribut>> Inventory.id:Long =>=>=> RelationalSchema.Column>> inventory.id PRIMARY KEY;
ClassDiagram.Attribut>> Inventory.quantity:int =>=>=> RelationalSchema.Column>> inventory.quantity;
ClassDiagram.Attribut>> Inventory.created_at:Date =>=>=> RelationalSchema.Column>> inventory.created_at;
ClassDiagram.Attribut>> Inventory._receipt:Date =>=>=> RelationalSchema.Column>> inventory._receipt;
ClassDiagram.Attribut>> Promotion.id:Long =>=>=> RelationalSchema.Column>> promotion.id PRIMARY KEY;
ClassDiagram.Attribut>> Promotion.name:String =>=>=> RelationalSchema.Column>> promotion.name;
ClassDiagram.Attribut>> Promotion.description:String =>=>=> RelationalSchema.Column>> promotion.description;
ClassDiagram.Attribut>> Promotion.sale_off:int =>=>=> RelationalSchema.Column>> promotion.sale_off;
ClassDiagram.Attribut>> Promotion.status:int =>=>=> RelationalSchema.Column>> promotion.status;
ClassDiagram.Attribut>> Promotion.created_at:Date =>=>=> RelationalSchema.Column>> promotion.created_at;
ClassDiagram.Attribut>> Promotion.start_time:Date =>=>=> RelationalSchema.Column>> promotion.start_time;
ClassDiagram.Attribut>> Promotion.end_time:Date =>=>=> RelationalSchema.Column>> promotion.end_time;
ClassDiagram.Attribut>> Ward.wardid:String =>=>=> RelationalSchema.Column>> ward.wardid PRIMARY KEY;
ClassDiagram.Attribut>> Ward.name:String =>=>=> RelationalSchema.Column>> ward.name;
ClassDiagram.Attribut>> Ward.districtid:String =>=>=> RelationalSchema.Column>> ward.districtid;
ClassDiagram.Attribut>> OrderDetail.id:OrderDetailId =>=>=> RelationalSchema.Column>> orderdetail.id;
ClassDiagram.Attribut>> OrderDetail.quantity:int =>=>=> RelationalSchema.Column>> orderdetail.quantity;
ClassDiagram.Attribut>> Users.id:Long =>=>=> RelationalSchema.Column>> users.id PRIMARY KEY;
ClassDiagram.Attribut>> Users.email:String =>=>=> RelationalSchema.Column>> users.email;
ClassDiagram.Attribut>> Users.password:String =>=>=> RelationalSchema.Column>> users.password;
ClassDiagram.Attribut>> Producer.id:Long =>=>=> RelationalSchema.Column>> producer.id PRIMARY KEY;
ClassDiagram.Attribut>> Producer.name:String =>=>=> RelationalSchema.Column>> producer.name;
ClassDiagram.Attribut>> Producer.status:int =>=>=> RelationalSchema.Column>> producer.status;
ClassDiagram.Attribut>> Producer.plug:String =>=>=> RelationalSchema.Column>> producer.plug;
ClassDiagram.Attribut>> Order.id:Long =>=>=> RelationalSchema.Column>> order.id PRIMARY KEY;
ClassDiagram.Attribut>> Order.address:String =>=>=> RelationalSchema.Column>> order.address;
ClassDiagram.Attribut>> Order.phone:String =>=>=> RelationalSchema.Column>> order.phone;
ClassDiagram.Attribut>> Order.created_at:Date =>=>=> RelationalSchema.Column>> order.created_at;
ClassDiagram.Attribut>> Category.id:Long =>=>=> RelationalSchema.Column>> category.id PRIMARY KEY;
ClassDiagram.Attribut>> Category.name:String =>=>=> RelationalSchema.Column>> category.name;
ClassDiagram.Attribut>> Category.plug:String =>=>=> RelationalSchema.Column>> category.plug;
ClassDiagram.Attribut>> Category.parentid:Long =>=>=> RelationalSchema.Column>> category.parentid;
ClassDiagram.Attribut>> Category.status:int =>=>=> RelationalSchema.Column>> category.status;
ClassDiagram.Attribut>> Material.id:Long =>=>=> RelationalSchema.Column>> material.id PRIMARY KEY;
ClassDiagram.Attribut>> Material.name:String =>=>=> RelationalSchema.Column>> material.name;
ClassDiagram.Attribut>> Material.plug:String =>=>=> RelationalSchema.Column>> material.plug;
ClassDiagram.Attribut>> Material.status:int =>=>=> RelationalSchema.Column>> material.status;
ClassDiagram.Attribut>> Origin.id:Long =>=>=> RelationalSchema.Column>> origin.id PRIMARY KEY;
ClassDiagram.Attribut>> Origin.name:String =>=>=> RelationalSchema.Column>> origin.name;
ClassDiagram.Attribut>> Origin.plug:String =>=>=> RelationalSchema.Column>> origin.plug;
ClassDiagram.Attribut>> Origin.status:int =>=>=> RelationalSchema.Column>> origin.status;
ClassDiagram.Attribut>> OrderGroup.id:Long =>=>=> RelationalSchema.Column>> ordergroup.id PRIMARY KEY;
ClassDiagram.Attribut>> OrderGroup.address:String =>=>=> RelationalSchema.Column>> ordergroup.address;
ClassDiagram.Attribut>> OrderGroup.phone:String =>=>=> RelationalSchema.Column>> ordergroup.phone;
ClassDiagram.Attribut>> OrderGroup.created_at:Date =>=>=> RelationalSchema.Column>> ordergroup.created_at;
One-To-Many relationship from ClassDiagram.Class>>OrderStatus  to ClassDiagram.Class>>List<Order>;
One-To-Many relationship from ClassDiagram.Class>>Color  to ClassDiagram.Class>>List<OrderDetail>;
One-To-Many relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>List<Inventory>;
One-To-Many relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>List<Question>;
One-To-Many relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>List<Image>;
One-To-Many relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>List<Image360>;
One-To-Many relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>List<OrderDetail>;
One-To-Many relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>List<Review>;
One-To-Many relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>List<UnitPrice>;
One-To-Many relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>List<OrderDetail>;
Many-To-One relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>Category represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>Store represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>Producer represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>origin represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>Product  to ClassDiagram.Class>>Material represented by ClassDiagram.Atrribute>>s;
Many-To-Many relationship between ClassDiagram.Class>>Product  and ClassDiagram.Class>>Color: product_color(product_id:Product [PK] #FK to Product,color_id:Color [PK] #FK to Color);
null: product_color(product_id:Product [PK] #FK to Product,color_id:Color [PK] #FK to Color);
Many-To-One relationship from ClassDiagram.Class>>Image360  to ClassDiagram.Class>>Product represented by ClassDiagram.Atrribute>>_id;
One-To-Many relationship from ClassDiagram.Class>>Province  to ClassDiagram.Class>>List<Store>;
One-To-Many relationship from ClassDiagram.Class>>District  to ClassDiagram.Class>>List<Store>;
Many-To-One relationship from ClassDiagram.Class>>Review  to ClassDiagram.Class>>Users represented by ClassDiagram.Atrribute>>user;
Many-To-One relationship from ClassDiagram.Class>>Review  to ClassDiagram.Class>>Product represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>Review  to ClassDiagram.Class>>Order represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>Image  to ClassDiagram.Class>>Product represented by ClassDiagram.Atrribute>>_id;
One-To-Many relationship from ClassDiagram.Class>>PaymentType  to ClassDiagram.Class>>Set<Order>;
One-To-Many relationship from ClassDiagram.Class>>PaymentType  to ClassDiagram.Class>>Set<OrderGroup>;
One-To-One relationship between ClassDiagram.Class>>PasswordResetToken  to ClassDiagram.Class>>Users represented by ClassDiagram.Atrribute>>user;
One-To-Many relationship from ClassDiagram.Class>>UnitPrice  to ClassDiagram.Class>>List<OrderDetail>;
Many-To-One relationship from ClassDiagram.Class>>UnitPrice  to ClassDiagram.Class>>Product represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>Answer  to ClassDiagram.Class>>Question represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>Answer  to ClassDiagram.Class>>Store represented by ClassDiagram.Atrribute>>s;
One-To-One relationship between ClassDiagram.Class>>Customer  to ClassDiagram.Class>>Users represented by ClassDiagram.Atrribute>>GeneratedName;
One-To-One relationship between ClassDiagram.Class>>Store  to ClassDiagram.Class>>Users represented by ClassDiagram.Atrribute>>GeneratedName;
One-To-Many relationship from ClassDiagram.Class>>Store  to ClassDiagram.Class>>List<Answer>;
One-To-Many relationship from ClassDiagram.Class>>Store  to ClassDiagram.Class>>List<Order>;
One-To-Many relationship from ClassDiagram.Class>>Store  to ClassDiagram.Class>>List<Product>;
One-To-Many relationship from ClassDiagram.Class>>Store  to ClassDiagram.Class>>List<Promotion>;
One-To-Many relationship from ClassDiagram.Class>>Store  to ClassDiagram.Class>>List<Member>;
Many-To-One relationship from ClassDiagram.Class>>Store  to ClassDiagram.Class>>Province represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>Store  to ClassDiagram.Class>>District represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>Store  to ClassDiagram.Class>>Ward represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>Member  to ClassDiagram.Class>>Member represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>Member  to ClassDiagram.Class>>Store represented by ClassDiagram.Atrribute>>s;
One-To-Many relationship from ClassDiagram.Class>>Question  to ClassDiagram.Class>>List<Answer>;
Many-To-One relationship from ClassDiagram.Class>>Question  to ClassDiagram.Class>>Product represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>Question  to ClassDiagram.Class>>Users represented by ClassDiagram.Atrribute>>user;
One-To-Many relationship from ClassDiagram.Class>>MemberType  to ClassDiagram.Class>>Set<Member>;
Many-To-One relationship from ClassDiagram.Class>>Inventory  to ClassDiagram.Class>>Product represented by ClassDiagram.Atrribute>>s;
One-To-Many relationship from ClassDiagram.Class>>Promotion  to ClassDiagram.Class>>List<OrderDetail>;
Many-To-One relationship from ClassDiagram.Class>>Promotion  to ClassDiagram.Class>>Store represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-Many relationship between ClassDiagram.Class>>Promotion  and ClassDiagram.Class>>Product: product_promotion(promotion_id:Promotion [PK] #FK to Promotion,product_id:Product [PK] #FK to Product);
One-To-Many relationship from ClassDiagram.Class>>Ward  to ClassDiagram.Class>>List<Store>;
Many-To-One relationship from ClassDiagram.Class>>OrderDetail  to ClassDiagram.Class>>Product represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>OrderDetail  to ClassDiagram.Class>>Order represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>OrderDetail  to ClassDiagram.Class>>Color represented by ClassDiagram.Atrribute>>s;
Many-To-One relationship from ClassDiagram.Class>>OrderDetail  to ClassDiagram.Class>>UnitPrice represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>OrderDetail  to ClassDiagram.Class>>Promotion represented by ClassDiagram.Atrribute>>GeneratedName;
One-To-One relationship between ClassDiagram.Class>>Users  to ClassDiagram.Class>>Store represented by ClassDiagram.Atrribute>>GeneratedName;
One-To-One relationship between ClassDiagram.Class>>Users  to ClassDiagram.Class>>Customer represented by ClassDiagram.Atrribute>>GeneratedName;
One-To-Many relationship from ClassDiagram.Class>>Users  to ClassDiagram.Class>>Set<Order>;
One-To-Many relationship from ClassDiagram.Class>>Users  to ClassDiagram.Class>>Set<OrderGroup>;
One-To-Many relationship from ClassDiagram.Class>>Users  to ClassDiagram.Class>>Set<Review>;
One-To-Many relationship from ClassDiagram.Class>>Users  to ClassDiagram.Class>>Set<Question>;
Many-To-Many relationship between ClassDiagram.Class>>Users  and ClassDiagram.Class>>Role: user_role(user_id:Users [PK] #FK to Users,role_id:Role [PK] #FK to Role);
One-To-Many relationship from ClassDiagram.Class>>Producer  to ClassDiagram.Class>>List<Product>;
One-To-Many relationship from ClassDiagram.Class>>Order  to ClassDiagram.Class>>List<OrderDetail>;
One-To-Many relationship from ClassDiagram.Class>>Order  to ClassDiagram.Class>>List<Review>;
Many-To-One relationship from ClassDiagram.Class>>Order  to ClassDiagram.Class>>PaymentType represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>Order  to ClassDiagram.Class>>Users represented by ClassDiagram.Atrribute>>user;
Many-To-One relationship from ClassDiagram.Class>>Order  to ClassDiagram.Class>>OrderStatus represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>Order  to ClassDiagram.Class>>Order represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>Order  to ClassDiagram.Class>>Store represented by ClassDiagram.Atrribute>>s;
One-To-Many relationship from ClassDiagram.Class>>Category  to ClassDiagram.Class>>List<Product>;
One-To-Many relationship from ClassDiagram.Class>>Material  to ClassDiagram.Class>>List<Product>;
One-To-Many relationship from ClassDiagram.Class>>Origin  to ClassDiagram.Class>>List<Product>;
One-To-Many relationship from ClassDiagram.Class>>OrderGroup  to ClassDiagram.Class>>List<Order>;
Many-To-One relationship from ClassDiagram.Class>>OrderGroup  to ClassDiagram.Class>>PaymentType represented by ClassDiagram.Atrribute>>GeneratedName;
Many-To-One relationship from ClassDiagram.Class>>OrderGroup  to ClassDiagram.Class>>Users represented by ClassDiagram.Atrribute>>user;
```


