# Geodes_dataset_part1
This directory shows the extraction of database schemas and class diagrams extracted via java programs (with JPA and/or Hibernate); in each directory you will find these files:

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
# Links
List of project : https://github.com/KhalidBelharbi/JPA-Hibernate-projects-on-Github

Part1: https://github.com/KhalidBelharbi/Geodes_dataset_part1/tree/master

Part2: https://github.com/KhalidBelharbi/Geodes_dataset_part2/tree/master

Part3: https://github.com/KhalidBelharbi/Geodes_dataset_part3/tree/master

# Exemple of Output
we can show the result obtained for the program which is below the link: https://github.com/anhtuangithub/2019_San-giao-dich-trang-tri-noi-that/tree/master/luanvan/src


## Git_Link.txt
```txt
Local Path: /u/belharbk/dataset/2019_San-giao-dich-trang-tri-noi-that/luanvan/src
Github Link:https://github.com/anhtuangithub/2019_San-giao-dich-trang-tri-noi-that/tree/master/luanvan/src
```
## allClasses.ecore
```xml
<?xml version="1.0" encoding="UTF-8"?>
<ecore:EPackage xmi:version="2.0" xmlns:xmi="http://www.omg.org/XMI" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:ecore="http://www.eclipse.org/emf/2002/Ecore" name="AllClasses" nsURI="file:/part/01/Tmp/belharbk/2019_San-giao-dich-trang-tri-noi-that/allClasses.xsd"
    nsPrefix="AllClasses">
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
  <eClassifiers xsi:type="ecore:EClass" name="Customuserdetails">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="customuserdetails"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="serialversionuid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="serialversionuid"/>
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
    <eStructuralFeatures xsi:type="ecore:EReference" name="grantedauthorities" lowerBound="1"
        eType="ecore:EClass http://www.eclipse.org/emf/2002/Ecore#//EObject" containment="true"
        resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="grantedauthorities"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="storeid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="storeid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="customerid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="customerid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="hethan" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//DateTime">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="hethan"/>
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
  <eClassifiers xsi:type="ecore:EClass" name="Mailconfig">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="mailconfig"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="beanPublicjavamailsendergetjavamailsenderJavamailsenderimplmailsender"
        lowerBound="1" eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//String">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="//@bean//publicjavamailsendergetjavamailsender(){//javamailsenderimplmailsender"/>
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
  <eClassifiers xsi:type="ecore:EClass" name="Methodsecurityconfig">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="methodsecurityconfig"/>
      <details key="kind" value="empty"/>
    </eAnnotations>
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
    <eStructuralFeatures xsi:type="ecore:EReference" name="id" eType="#//Orderdetailid"
        unsettable="true" containment="true" resolveProxies="false">
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
  <eClassifiers xsi:type="ecore:EClass" name="Orderdetailid">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="orderdetailid"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="serialversionuid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="/***/serialversionuid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="orderid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="orderid"/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
    <eStructuralFeatures xsi:type="ecore:EAttribute" name="productid" lowerBound="1"
        eType="ecore:EDataType http://www.eclipse.org/emf/2003/XMLType#//Long" unsettable="true">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value="productid"/>
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
  <eClassifiers xsi:type="ecore:EClass" name="Storerepository">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="storerepository"/>
      <details key="kind" value="empty"/>
    </eAnnotations>
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
  <eClassifiers xsi:type="ecore:EClass" name="Webmvcconfig">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="webmvcconfig"/>
      <details key="kind" value="empty"/>
    </eAnnotations>
  </eClassifiers>
  <eClassifiers xsi:type="ecore:EClass" name="Websecurityconfig">
    <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
      <details key="name" value="websecurityconfig"/>
      <details key="kind" value="elementOnly"/>
    </eAnnotations>
    <eStructuralFeatures xsi:type="ecore:EReference" name="_" lowerBound="1" eType="ecore:EClass http://www.eclipse.org/emf/2002/Ecore#//EObject"
        containment="true" resolveProxies="false">
      <eAnnotations source="http:///org/eclipse/emf/ecore/util/ExtendedMetaData">
        <details key="kind" value="element"/>
        <details key="name" value=""/>
        <details key="namespace" value="##targetNamespace"/>
      </eAnnotations>
    </eStructuralFeatures>
  </eClassifiers>
</ecore:EPackage>

```
## allClasses.xsd 
```txt
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<xs:schema version="1.0" xmlns:xs="http://www.w3.org/2001/XMLSchema">
   <xs:complexType name="orderstatus" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="color" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="orderdetails" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="product" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="description" type="xs:string" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="avatar" type="xs:string" />
        <xs:element name="avgstart" type="xs:double" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="upd_at" type="xs:dateTime" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="inventory" type="inventory" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="questions" type="question" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="images" type="image" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="image360" type="image360" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="orderdetails" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="reviews" type="review" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="unitprices" type="unitprice" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="s" type="category" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
        <xs:element name="s" type="producer" nillable="true" minOccurs="0" />
        <xs:element name="s" type="origin" nillable="true" minOccurs="0" />
        <xs:element name="s" type="material" nillable="true" minOccurs="0" />
        <xs:element name="colors" type="color" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="promotions" type="promotion" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="image360" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="path" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="_id" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="province" >
      <xs:sequence>
        <xs:element name="provinceid" type="xs:string" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="stores" type="store" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="district" >
      <xs:sequence>
        <xs:element name="districtid" type="xs:string" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="provinceid" type="xs:string" />
        <xs:element name="stores" type="store" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="review" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="rating" type="xs:long" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="upd_at" type="xs:dateTime" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="s" type="product" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="order" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="image" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="path" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="_id" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="paymenttype" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="ordergroup" type="ordergroup" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="passwordresettoken" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="token" type="xs:string" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="expiry" type="xs:dateTime" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="unitprice" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="price" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="start_time" type="xs:dateTime" />
        <xs:element name="end_time" type="xs:dateTime" />
        <xs:element name="root" type="xs:long" />
        <xs:element name="orderdetails" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="answer" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="s" type="question" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderdetailid" >
      <xs:sequence>
        <xs:element name="/***/serialversionuid" type="xs:long" />
        <xs:element name="orderid" type="xs:long" />
        <xs:element name="productid" type="xs:long" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="customer" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="sex" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="birthday" type="xs:dateTime" />
        <xs:element name="GeneratedName" type="users" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="store" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="introduce" type="xs:string" />
        <xs:element name="website" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="GeneratedName" type="users" nillable="true" minOccurs="0" />
        <xs:element name="answers" type="answer" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="promotions" type="promotion" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="members" type="member" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="province" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="district" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="ward" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="member" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="start_time" type="xs:dateTime" />
        <xs:element name="end_time" type="xs:dateTime" />
        <xs:element name="s" type="membertype" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="question" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="answers" type="answer" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="s" type="product" nillable="true" minOccurs="0" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="membertype" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="price" type="xs:long" />
        <xs:element name="members" type="member" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="role" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="users" type="users" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="inventory" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="_receipt" type="xs:dateTime" />
        <xs:element name="s" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="promotion" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="description" type="xs:string" />
        <xs:element name="sale_off" type="xs:long" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="start_time" type="xs:dateTime" />
        <xs:element name="end_time" type="xs:dateTime" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="store" nillable="true" minOccurs="0" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="customuserdetails" >
      <xs:complexContent>
       <xs:extension base="grantedauthority>">
         <xs:sequence>
          <xs:element name="serialversionuid" type="xs:long" />
          <xs:element name="user" type="users" nillable="true" minOccurs="0" />
          <xs:element name="grantedauthorities" type="xs:anyType" />
          <xs:element name="storeid" type="xs:long" />
          <xs:element name="customerid" type="xs:long" />
          <xs:element name="hethan" type="xs:dateTime" />
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ward" >
      <xs:sequence>
        <xs:element name="wardid" type="xs:string" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="districtid" type="xs:string" />
        <xs:element name="stores" type="store" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderdetail" >
      <xs:sequence>
        <xs:element name="id" type="orderdetailid" nillable="true" minOccurs="0" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="GeneratedName" type="product" nillable="true" minOccurs="0" />
        <xs:element name="s" type="order" nillable="true" minOccurs="0" />
        <xs:element name="s" type="color" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="unitprice" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="promotion" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="users" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="email" type="xs:string" />
        <xs:element name="password" type="xs:string" />
        <xs:element name="GeneratedName" type="store" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="customer" nillable="true" minOccurs="0" />
        <xs:element name="order" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="ordergroup" type="ordergroup" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="reviews" type="review" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="questions" type="question" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="roles" type="role" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="producer" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="order" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="review" type="review" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="paymenttype" nillable="true" minOccurs="0" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="orderstatus" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="ordergroup" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="category" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="parentid" type="xs:long" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="product" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="material" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="origin" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ordergroup" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="paymenttype" nillable="true" minOccurs="0" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mailconfig" >
      <xs:sequence>
        <xs:element name="//@bean//publicjavamailsendergetjavamailsender(){//javamailsenderimplmailsender" type="xs:string" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="webmvcconfig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="websecurityconfig" >
      <xs:complexContent>
       <xs:extension base="websecurityconfigureradapter">
         <xs:sequence>
          <xs:element name="" type="xs:anyType" />
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="methodsecurityconfig" >
      <xs:complexContent>
       <xs:extension base="globalmethodsecurityconfiguration">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="storerepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<store,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="materialrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<material,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="inventoryrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<inventory,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ordergrouprepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<ordergroup,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="questionrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<question,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="memberrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<member,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="productrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<product,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="wardreponsitory" >
      <xs:complexContent>
       <xs:extension base="jparepository<ward,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="districtreponsitory" >
      <xs:complexContent>
       <xs:extension base="jparepository<district,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="categoryrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<category,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="rolerepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<role,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="customerrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<customer,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="orderrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<order,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="colorrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<color,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="passwordresettokenrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<passwordresettoken,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="producerrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<producer,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="promotionrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<promotion,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="orderstatusrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<orderstatus,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="orderdetailrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<orderdetail,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="answerrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<answer,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="provincereponsitory" >
      <xs:complexContent>
       <xs:extension base="jparepository<province,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="image360repository" >
      <xs:complexContent>
       <xs:extension base="jparepository<image360,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="reviewrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<review,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="unitpricerepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<unitprice,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="usersrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<users,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="membertyperepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<membertype,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="originrepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<origin,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="imagerepository" >
      <xs:complexContent>
       <xs:extension base="jparepository<image,">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="questioncontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="questionservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="categorycontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="categoryservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="origincontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="originservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="userscontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="usersservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="answercontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="answerservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="reviewcontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="reviewservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sendgridemailcontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="sendgridmailservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="colorcontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="colorservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="materialcontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="materialservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="provincecontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="provinceservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ordercontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="orderservice" nillable="true" minOccurs="0" />
        <xs:element name="dongabank" type="xs:string" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="promotioncontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="promotionservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="wardcontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="wardservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="membertypecontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="membertypeservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="productcontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="productservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="districtcontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="districtservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderstatuscontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="orderstatusservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="membercontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="memberservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="producercontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="producerservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="storecontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="storeservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rolecontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="roleservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="customercontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="customerservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="promotionproductdto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="description" type="xs:string" />
        <xs:element name="sale_off" type="xs:long" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="create_at" type="xs:dateTime" />
        <xs:element name="start_time" type="xs:dateTime" />
        <xs:element name="end_time" type="xs:dateTime" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="testdto" >
      <xs:sequence>
        <xs:element name="email" type="xs:string" />
        <xs:element name="password" type="xs:string" />
        <xs:element name="rolelist" type="role" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ordergroupdto" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="ordergroup" nillable="true" minOccurs="0" />
        <xs:element name="orderdto" type="orderdto" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="roleuserdto" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderdetaildto" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="product" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="promotion" nillable="true" minOccurs="0" />
        <xs:element name="quantity" type="xs:long" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="productdto" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="product" nillable="true" minOccurs="0" />
        <xs:element name="colors" type="color" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="resetpassworddto" >
      <xs:sequence>
        <xs:element name="email" type="xs:string" />
        <xs:element name="password" type="xs:string" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="storedto" >
      <xs:sequence>
        <xs:element name="email" type="xs:string" />
        <xs:element name="password" type="xs:string" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderdto" >
      <xs:sequence>
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="GeneratedName" type="paymenttype" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
        <xs:element name="ordersdetaildto" type="orderdetaildto" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="customerdto" >
      <xs:sequence>
        <xs:element name="email" type="xs:string" />
        <xs:element name="password" type="xs:string" />
        <xs:element name="s" type="customer" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cartdto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="quantity" type="xs:long" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="topseller" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderadmindto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="GeneratedName" type="paymenttype" nillable="true" minOccurs="0" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="orderstatus" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderdetaildto" >
      <xs:sequence>
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="total" type="xs:long" />
        <xs:element name="GeneratedName" type="unitprice" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="promotion" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="productadmindto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="avatar" type="xs:string" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="s" type="category" nillable="true" minOccurs="0" />
        <xs:element name="s" type="producer" nillable="true" minOccurs="0" />
        <xs:element name="s" type="origin" nillable="true" minOccurs="0" />
        <xs:element name="s" type="material" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
        <xs:element name="unitprices" type="unitprice" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="listexchange" >
      <xs:sequence>
        <xs:element name="items" type="item" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="reviewdto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="rating" type="xs:long" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="chartmonthbyyeardto" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="infoorderrecentdto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="GeneratedName" type="orderstatus" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="paymenttype" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="storedtoresponse" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="website" type="xs:string" />
        <xs:element name="introduce" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="GeneratedName" type="users" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="province" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="district" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="ward" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="reviewaccountdto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="rating" type="xs:long" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="s" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="imagedtoresponse" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="path" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="_id" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="userdto" >
      <xs:sequence>
        <xs:element name="email" type="xs:string" />
        <xs:element name="GeneratedName" type="store" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="customer" nillable="true" minOccurs="0" />
        <xs:element name="roles" type="role" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ordergroupresponsedto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="GeneratedName" type="paymenttype" nillable="true" minOccurs="0" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="questionresponsedto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="answers" type="answer" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="s" type="product" nillable="true" minOccurs="0" />
        <xs:element name="status" type="xs:long" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="item" >
      <xs:sequence>
        <xs:element name="type" type="xs:string" />
        <xs:element name="imageurl" type="xs:string" />
        <xs:element name="muatienmat" type="xs:string" />
        <xs:element name="muack" type="xs:string" />
        <xs:element name="bantienmat" type="xs:string" />
        <xs:element name="banck" type="xs:string" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="customerresponsedto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="sex" type="xs:string" />
        <xs:element name="birthday" type="xs:dateTime" />
        <xs:element name="GeneratedName" type="users" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="productdetaildto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="avatar" type="xs:string" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="avgstart" type="xs:double" />
        <xs:element name="description" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="unitprices" type="unitprice" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="promotions" type="promotion" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="s" type="producer" nillable="true" minOccurs="0" />
        <xs:element name="s" type="origin" nillable="true" minOccurs="0" />
        <xs:element name="s" type="material" nillable="true" minOccurs="0" />
        <xs:element name="colors" type="color" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
        <xs:element name="s" type="category" nillable="true" minOccurs="0" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="infouserdto" >
      <xs:sequence>
        <xs:element name="email" type="xs:string" />
        <xs:element name="GeneratedName" type="store" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="customer" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="productpromotiondto" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="avatar" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="avgstart" type="xs:double" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="unitprices" type="unitprice" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="buyquantity" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="promotions" type="promotion" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="colorservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="materialservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="usersservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="categoryservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="originservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="productservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="promotionservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="isecurityuserservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="storeservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="memberservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="districtserviceimpl" >
      <xs:sequence>
        <xs:element name="districtrepository" type="districtreponsitory" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="questionserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="questionrepository" nillable="true" minOccurs="0" />
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="storerepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="usersserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="rolerepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="customerrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="storerepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="memberrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="membertyperepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="passwordresettokenrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="sendgridmailservice" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="xs:anyType" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="userdetailsserviceimpl" >
      <xs:sequence>
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="memberrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="materialserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="materialrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sendgridmailserviceimpl" >
      <xs:sequence>
        <xs:element name="fromnoithat246" type="xs:string" />
        <xs:element name="client" type="xs:anyType" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="memberserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="memberrepository" nillable="true" minOccurs="0" />
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="storerepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="membertyperepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="promotionserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="promotionrepository" nillable="true" minOccurs="0" />
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="storerepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="categoryserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="categoryrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="wardserviceimpl" >
      <xs:sequence>
        <xs:element name="wardrepository" type="wardreponsitory" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="storeserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="storerepository" nillable="true" minOccurs="0" />
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="sendgridmailservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="colorserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="colorrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="customerserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="customerrepository" nillable="true" minOccurs="0" />
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderserviceimpl" >
      <xs:sequence>
        <xs:element name="url_formmail" type="xs:string" />
        <xs:element name="GeneratedName" type="orderrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="productrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="orderdetailrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="unitpricerepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="orderstatusrepository" nillable="true" minOccurs="0" />
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="storerepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="ordergrouprepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="sendgridmailservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="isecurityuserserviceimpl" >
      <xs:sequence>
        <xs:element name="passwordtokenrepository" type="passwordresettokenrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="provinceserviceimpl" >
      <xs:sequence>
        <xs:element name="provincerepository" type="provincereponsitory" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="membertypeserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="membertyperepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="originserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="originrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderstatusserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="orderstatusrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="reviewserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="reviewrepository" nillable="true" minOccurs="0" />
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="productrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="storerepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="roleserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="rolerepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="producerserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="producerrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="answerserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="answerrepository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="productserviceimpl" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="productrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="unitpricerepository" nillable="true" minOccurs="0" />
        <xs:element name="userrepository" type="usersrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="storerepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="imagerepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="inventoryrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="image360repository" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="wardservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="reviewservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderstatusservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="customerservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="membertypeservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sendgridmailservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="answerservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="roleservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="provinceservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="producerservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="questionservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="districtservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="locationapiapplication" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="errormessage" >
      <xs:sequence>
        <xs:element name="message" type="xs:string" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="notfoundexception" >
      <xs:complexContent>
       <xs:extension base="runtimeexception{">
         <xs:sequence>
          <xs:element name="/***/serialversionuid" type="xs:long" />
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="apiexceptionhandler" >
      <xs:complexContent>
       <xs:extension base="responseentityexceptionhandler">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="storepage" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="adminpage" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="homepagecontroller" >
      <xs:sequence>
        <xs:element name="GeneratedName" type="membertyperepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="originrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="producerrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="materialrepository" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="categorycontroller" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="categoryrepository" nillable="true" minOccurs="0" />
        <xs:element name="productsevice" type="productservice" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="orderservice" nillable="true" minOccurs="0" />
        <xs:element name="securityuserservice" type="isecurityuserservice" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-customer" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-order-destroy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-producer" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-orderstatus" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-category" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-material" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-store" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-color" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manage-origin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="roleservice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="page-best-seller" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="side-bar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="layout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="header" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="list-product-category-parent" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="page-product-random" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="product-of-store" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="login" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dang-ki-thanh-vien" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="list-product-promotion" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="account-manage-info" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="account-review" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="list-product-category" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="update-password" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="template" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="form-dang-ki" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="account-store" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="checkout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="addtocart" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="loadding" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bump" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="shell" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="changelog" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="clean" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vectormult" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vectoradd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vectorsubtract" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="setcolors" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rgbtoarray" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vectortonum" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vectorlength" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="arraytorgb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="unhighlight" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getpin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="selectindex" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="setscalecolors" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="setvalues" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="setnormalizefunction" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="resize" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="isselected" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="applytransform" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="reset" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="removepin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="setscale" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="colorscale" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.vmap.sampledata" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.vmap.turkey" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="continent" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="syria" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="new-york" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".eslintrc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="logo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="style" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-multiple" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-single-xy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-single" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-max" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-no-overlap" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-stacked" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-absolute" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-min-interval" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-offset" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-flex-offset" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bar-thickness-flex" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-radar-boundary-origin-spline" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-dataset-span" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-dataset-spline" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-origin-stepped-span" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-origin-span" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-end-span" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-start" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-origin-spline-span" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-origin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-end" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-radar-boundary-origin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-origin-spline" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-dataset" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-dataset-spline-span" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-start-span" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fill-line-boundary-origin-stepped" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="label-offset-vertical-axes" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="composer" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="book" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="icomoon" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="argentina" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="france" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="south-africa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="brazil" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="styled_maps" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gmaps.geofences" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gmaps.map_types" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gmaps.styles" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jasmine-gmaps" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="style" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gmaps.min.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jsdoc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="animate" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="animate.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slideinleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slideindown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slideinright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slideinup" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateoutdownright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateoutupright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateoutupleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateoutdownleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="wobble" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="heartbeat" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flash" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounce" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="swing" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rubberband" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tada" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="headshake" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="shake" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jello" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pulse" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceoutdown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceoutright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceoutleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceoutup" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateindownleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotatein" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateinupleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateinupright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotateindownright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_base" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flip" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flipouty" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flipiny" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flipinx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flipoutx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeoutrightbig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeoutupbig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeoutleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeoutdown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeoutleftbig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeoutright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeoutup" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeoutdownbig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slideoutup" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slideoutright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slideoutleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slideoutdown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoominup" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoominright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoominleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoomindown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoomin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeindown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeindownbig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeinleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeinrightbig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeinup" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeinupbig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeinleftbig" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadein" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fadeinright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceinleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceinright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceindown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bouncein" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bounceinup" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hinge" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jackinthebox" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rollin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rollout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoomoutup" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoomoutleft" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoomoutright" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoomoutdown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zoomout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lightspeedout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lightspeedin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package-lock" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="animate-config" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_bg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_zh.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_eu.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fr.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_da" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sr_lat" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ja" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_zh_tw.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ca.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_az.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ka.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sl.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_gl.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_az" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_bg.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pt_pt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sv.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es_pe.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_uk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sr_lat.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ro" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ja.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es_ar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_zh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fa.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es_ar.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ka" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_th" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_nl.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pt_br.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_si" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_mk.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hy_am.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_no" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_lv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_uk.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_de" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_cs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_is.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_lt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hu.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ge.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_et" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_eu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_tj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pt_br" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_gl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_id.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_nl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hy_am" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sr.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ge" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_is" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pl.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ur" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_da.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_kk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_id" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_lv.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sk.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_kk.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_bn_bd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ru.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_cs.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es_pe" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_si.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_lt.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ur.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_no.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sd.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ar.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ro.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_my" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_de.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_zh_tw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_th.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_mk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_el" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_et.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_tr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ko.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_tr.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_he" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_vi.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_it.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fi.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_it" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hr.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ru" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_my.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pt_pt.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_tj.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_el.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ko" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_bn_bd.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_vi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery-validation-sri" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="validation.jquery" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gruntfile" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ajax" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bic" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="maxfiles" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="giroaccountnl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="notequalto" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nippl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="maxsize" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="greaterthanequal" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="require_from_group" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lessthan" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pattern" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lettersonly" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="skip_or_fill_minimum" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nifes" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="greaterthan" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="maxsizetotal" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="strippedminlength" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="extension" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lessthanequal" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="iban" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bankorgiroaccountnl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="currency" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="statesus" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bankaccountnl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vinus" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="niees" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_vi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ko" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_mk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_el" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pt_pt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ru" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_it" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_tr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_he" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es_ar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_my" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_is" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ur" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ge" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_pt_br" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_kk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_hy_am" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_id" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_et" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_de" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_cs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_lt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sr_lat" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_nl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_tj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_eu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_gl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_th" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_bn_bd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ro" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es_pe" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_fi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ka" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_zh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_no" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_lv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_si" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_zh_tw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_az" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_sl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_es" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_uk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_bg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ja" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="messages_da" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="svgo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ba" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ly" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ax" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="es-ct" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ec" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="aq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="am" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ad" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ru" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ki" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="uy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="wf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="st" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="md" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ss" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="iq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb-sct" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb-nir" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="no" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ws" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="id" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="de" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ci" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb-wls" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ye" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="td" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="na" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="so" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="im" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ae" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="va" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="br" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="al" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="um" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ee" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="aw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ro" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="il" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="si" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="my" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ng" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb-eng" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ie" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="py" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ni" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ch" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="co" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mp" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pe" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ga" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ml" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="za" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="me" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ps" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gp" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="io" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="to" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ms" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="th" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ck" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ge" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="it" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ph" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="is" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ma" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="es" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="et" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="af" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ve" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="li" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ke" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ao" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="at" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="re" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ky" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="un" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="as" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kp" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="az" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ug" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ir" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="yt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="je" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="np" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="se" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jp" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="in" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="do" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ne" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="be" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ua" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="om" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ls" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="au" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="us" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="qa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ai" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ag" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ht" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="by" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="uz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="km" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="er" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="la" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="se" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ne" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="do" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="in" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jp" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb-eng" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ir" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="np" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="je" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="yt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ai" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="qa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="us" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="er" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="la" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="km" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="uz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="by" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ag" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ht" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ua" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="be" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="au" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ls" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="om" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ge" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb-wls" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ma" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="is" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ph" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="it" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="io" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb-sct" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gp" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ps" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gb-nir" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ck" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="th" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ms" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="to" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="as" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="un" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ky" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="re" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="at" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ug" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="az" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kp" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ve" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="af" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="et" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="es" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ao" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ke" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="li" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="aw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ee" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="um" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ro" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="va" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ae" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="al" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="br" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ml" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ga" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pe" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="me" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="za" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ng" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="my" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="si" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="il" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mp" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="co" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ch" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ni" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="py" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mw" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ie" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="am" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="es-ct" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="uy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ki" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ru" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ad" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ax" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ly" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ba" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="kr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="aq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ec" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ci" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tj" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="de" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="id" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ws" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="no" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="im" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="so" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="na" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="td" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ye" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="iq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ss" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="md" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="st" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="wf" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sz" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mm" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flag-icon.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flag-icon" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="composer" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flag-icon-base" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flag-icon-list" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flag-icon-more" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flag-icon" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_flag-icon-more" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_flag-icon-list" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_breadcrumb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_transitions" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_mixins" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_carousel" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_jumbotron" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_reboot" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_tooltip" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_media" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_grid" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_close" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_background" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_clearfix" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_visibility" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_shadows" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_align" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_screenreaders" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_embed" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_card" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_dropdown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_progress" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_button-group" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_list-group" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-reboot" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_images" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_code" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_nav" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_pagination" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_functions" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_type" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_print" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_utilities" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_input-group" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-grid" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_hover" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_buttons" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_image" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_alert" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_float" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_visibility" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_breakpoints" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_lists" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_resize" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_transition" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_badge" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_box-shadow" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_nav-divider" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_caret" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_text-hide" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_grid" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_screen-reader" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_text-truncate" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_border-radius" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_size" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_gradients" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_clearfix" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_pagination" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_reset-text" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:complexContent>
       <xs:extension base="">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name=".eslintrc" >
      <xs:complexContent>
       <xs:extension base="">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="button.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dropdown.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tab.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tooltip.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="alert.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="popover.js" >
      <xs:complexContent>
       <xs:extension base="tooltip">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="modal.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="scrollspy.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="util.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="collapse.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="carousel.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="alert" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".eslintrc" >
      <xs:complexContent>
       <xs:extension base="">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="sache" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-grid.css" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap.min.css" >
      <xs:complexContent>
       <xs:extension base="the">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="bootstrap.css" >
      <xs:complexContent>
       <xs:extension base="the">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="bootstrap-grid.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-reboot.min.css" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-reboot.css" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-grid.min.css" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-grid" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap.js" >
      <xs:complexContent>
       <xs:extension base="tooltip">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="bootstrap.bundle.min.js" >
      <xs:complexContent>
       <xs:extension base="keeptogether">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="bootstrap.min.js" >
      <xs:complexContent>
       <xs:extension base="tooltip">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="bootstrap.bundle.js" >
      <xs:complexContent>
       <xs:extension base="keeptogether">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bug" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bug_report" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gemfile" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="colors" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="breakpoints" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="examples" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="theme-colors" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="grays" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="manifest" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="safari-pinned-tab" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="docs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_examples" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_anchor" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_browser-bugs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_masthead" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_content" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-solid" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-punchout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap-outline" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="docs.min.css" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pwa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".eslintrc" >
      <xs:complexContent>
       <xs:extension base="">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="starter-template" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="navbar-top" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".eslintrc" >
      <xs:complexContent>
       <xs:extension base="">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="grid" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jumbotron" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cover" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="form-validation" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="navbar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="navbar-top-fixed" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pricing" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:complexContent>
       <xs:extension base="">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="callout" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="callout-info-mediaqueries-breakpoints" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="social" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="import" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slack" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="twitter" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="menu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bootstrap" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="download" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lightning" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="github" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="footer" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="favicons" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="skippy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ads" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="docs-navbar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="simple" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="examples" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="docs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="default" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="home" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package-lock" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="composer" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cname" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="popper.js" >
      <xs:complexContent>
       <xs:extension base="keeptogether">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="popper-utils.min.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="popper-utils.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="popper.min.js" >
      <xs:complexContent>
       <xs:extension base="keeptogether">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="popper-utils.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="popper.js" >
      <xs:complexContent>
       <xs:extension base="keeptogether">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="popper-utils.min.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="popper.min.js" >
      <xs:complexContent>
       <xs:extension base="keeptogether">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="popper-utils.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="popper.js" >
      <xs:complexContent>
       <xs:extension base="keeptogether">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="popper.min.js" >
      <xs:complexContent>
       <xs:extension base="keeptogether">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="popper-utils.min.js" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="example20t-code" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="default" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="page" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="page-nowrap" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tooltip-examples" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tooltip-documentation" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_functions" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="popper-documentation" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cname" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="documentation" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.scrolly.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.scrollex.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getoutersizes" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getstylecomputedproperty" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ismodifierenabled" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="find" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getwindow" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="setattributes" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getclientrect" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getroot" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="then" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="simulatescroll" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getrect" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="prepend" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lerna" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="font-awesome.css" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fixed-width" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="animated" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="stacked" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mixins" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bordered-pulled" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="core" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="screen-reader" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rotated-flipped" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="list" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="larger" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="font-awesome" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="icons" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_screen-reader" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="font-awesome" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="composer" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="buttons.bootstrap4.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="contributing" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package-lock" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="build" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="version" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="component" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="flot.jquery" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.flot.pie" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.flot.fillbetween" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery-ui.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data-japan-gdp-growth" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data-eu-gdp-growth-4" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data-usa-gdp-growth" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data-eu-gdp-growth-5" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data-eu-gdp-growth-1" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data-eu-gdp-growth" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data-eu-gdp-growth-3" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data-eu-gdp-growth-2" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:complexContent>
       <xs:extension base="to">
         <xs:sequence>
         </xs:sequence>
       </xs:extension>
      </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".travis" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="composer" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="charts" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="style" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="show" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".travis" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gemfile" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="licence" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="adjustcss" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="support" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="showhide" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="defaultdisplay" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="curcss" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="addgethookif" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hiddenvisibleselectors" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ishidden" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cssexpand" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getstyles" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rnumnonpx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rmargin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="swap" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="push" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="class2type" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="support" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rcssnum" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="concat" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hasown" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="arr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="slice" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tostring" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="document" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="indexof" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="documentelement" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="support" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="prop" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="datapriv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="datauser" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="acceptdata" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="selector-sizzle" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="deferred" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="queue" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="effects" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="css" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="load" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nonce" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="location" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="xhr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="parsexml" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="parsejson" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="alias" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="trigger" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ajax" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="support" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="focusin" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="wrap" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="animatedselector" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tween" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="deprecated" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rneedscontext" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dir" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="siblings" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="offset" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="selector" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="amd" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="global" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="intro" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="outro" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="traversing" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="attributes" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="callbacks" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ready" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="parsehtml" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="access" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_evalurl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="wrapmap" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="support" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="setglobaleval" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="getall" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rcheckabletype" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="delay" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dimensions" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sizzle.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="datatables.bootstrap4.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="datatables.bootstrap4" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package-lock" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="package" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="component" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jszip_utils" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fetch_api" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="download-zip-file" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="downloader" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="read-local-file-api" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="downloader" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="helpers" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="blob" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="blob" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data_uri" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="data_uri" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="read" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="readable-stream-browser" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license_header" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="references" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name=".bower" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="themify" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="config" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fontello" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fulltoolbareditor" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="replacebyclass" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sample_posteddata" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="posteddata" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="languages" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="logo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="et" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="de" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="no" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="si" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="th" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ro" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="es-mx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="az" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fr-ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ja" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sr-latn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pt-br" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_translationstatus" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="da" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="af" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="en" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="it" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="km" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="he" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="el" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="en-au" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zh-cn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ug" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="mn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="oc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="id" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="de-ch" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="en-gb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="anchor" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zh" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ro" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="th" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="en-au" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="_translationstatus" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="si" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="no" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="lt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cs" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="de" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="et" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="gl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ku" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="bg" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="de-ch" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="en-gb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="da" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ja" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="az" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="uk" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="es" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="zh-cn" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ar" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="es-mx" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="el" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="en-ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="he" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tr" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pl" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="km" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="nb" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="it" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ru" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ko" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="vi" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="eo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="en" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sq" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="af" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="id" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="tt" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="pt-br" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="oc" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="hu" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="sv" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fr-ca" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="fa" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ug" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="cy" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="license" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="dialogdefinition" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rescarousel.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="toastr.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ng-ckeditor.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="style.css" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="index" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.rateyo.min" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="jquery.rateyo" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="util" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="rescarousel" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="locationapiapplicationtests" >
      <xs:sequence>
      </xs:sequence>
   </xs:complexType>
</xs:schema> 
```
## DomainModel.ecore
```txt
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
## DomainModel.xsd
```txt
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<xs:schema version="1.0" xmlns:xs="http://www.w3.org/2001/XMLSchema">
   <xs:complexType name="orderstatus" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="color" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="orderdetails" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="product" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="description" type="xs:string" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="avatar" type="xs:string" />
        <xs:element name="avgstart" type="xs:double" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="upd_at" type="xs:dateTime" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="inventory" type="inventory" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="questions" type="question" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="images" type="image" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="image360" type="image360" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="orderdetails" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="reviews" type="review" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="unitprices" type="unitprice" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="s" type="category" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
        <xs:element name="s" type="producer" nillable="true" minOccurs="0" />
        <xs:element name="s" type="origin" nillable="true" minOccurs="0" />
        <xs:element name="s" type="material" nillable="true" minOccurs="0" />
        <xs:element name="colors" type="color" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="promotions" type="promotion" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="image360" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="path" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="_id" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="province" >
      <xs:sequence>
        <xs:element name="provinceid" type="xs:string" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="stores" type="store" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="district" >
      <xs:sequence>
        <xs:element name="districtid" type="xs:string" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="provinceid" type="xs:string" />
        <xs:element name="stores" type="store" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="review" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="rating" type="xs:long" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="upd_at" type="xs:dateTime" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="s" type="product" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="order" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="image" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="path" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="_id" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="paymenttype" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="ordergroup" type="ordergroup" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="passwordresettoken" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="token" type="xs:string" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="expiry" type="xs:dateTime" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="unitprice" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="price" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="start_time" type="xs:dateTime" />
        <xs:element name="end_time" type="xs:dateTime" />
        <xs:element name="root" type="xs:long" />
        <xs:element name="orderdetails" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="answer" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="s" type="question" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="customer" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="sex" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="birthday" type="xs:dateTime" />
        <xs:element name="GeneratedName" type="users" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="store" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="introduce" type="xs:string" />
        <xs:element name="website" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="GeneratedName" type="users" nillable="true" minOccurs="0" />
        <xs:element name="answers" type="answer" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="promotions" type="promotion" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="members" type="member" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="province" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="district" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="ward" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="member" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="start_time" type="xs:dateTime" />
        <xs:element name="end_time" type="xs:dateTime" />
        <xs:element name="s" type="membertype" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="question" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="content" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="answers" type="answer" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="s" type="product" nillable="true" minOccurs="0" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="membertype" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="price" type="xs:long" />
        <xs:element name="members" type="member" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="role" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="users" type="users" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="inventory" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="_receipt" type="xs:dateTime" />
        <xs:element name="s" type="product" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="promotion" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="description" type="xs:string" />
        <xs:element name="sale_off" type="xs:long" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="start_time" type="xs:dateTime" />
        <xs:element name="end_time" type="xs:dateTime" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="store" nillable="true" minOccurs="0" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ward" >
      <xs:sequence>
        <xs:element name="wardid" type="xs:string" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="districtid" type="xs:string" />
        <xs:element name="stores" type="store" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="orderdetail" >
      <xs:sequence>
        <xs:element name="id" type="orderdetailid" nillable="true" minOccurs="0" />
        <xs:element name="quantity" type="xs:long" />
        <xs:element name="GeneratedName" type="product" nillable="true" minOccurs="0" />
        <xs:element name="s" type="order" nillable="true" minOccurs="0" />
        <xs:element name="s" type="color" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="unitprice" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="promotion" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="users" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="email" type="xs:string" />
        <xs:element name="password" type="xs:string" />
        <xs:element name="GeneratedName" type="store" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="customer" nillable="true" minOccurs="0" />
        <xs:element name="order" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="ordergroup" type="ordergroup" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="reviews" type="review" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="questions" type="question" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="roles" type="role" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="producer" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="order" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="orderdetail" type="orderdetail" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="review" type="review" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="paymenttype" nillable="true" minOccurs="0" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="orderstatus" nillable="true" minOccurs="0" />
        <xs:element name="GeneratedName" type="ordergroup" nillable="true" minOccurs="0" />
        <xs:element name="s" type="store" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="category" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="parentid" type="xs:long" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="product" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="material" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="origin" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="name" type="xs:string" />
        <xs:element name="plug" type="xs:string" />
        <xs:element name="status" type="xs:long" />
        <xs:element name="products" type="product" nillable="true" minOccurs="0" maxOccurs="unbounded" />
      </xs:sequence>
   </xs:complexType>
   <xs:complexType name="ordergroup" >
      <xs:sequence>
        <xs:element name="id" type="xs:long" />
        <xs:element name="address" type="xs:string" />
        <xs:element name="phone" type="xs:string" />
        <xs:element name="created_at" type="xs:dateTime" />
        <xs:element name="orders" type="order" nillable="true" minOccurs="0" maxOccurs="unbounded" />
        <xs:element name="GeneratedName" type="paymenttype" nillable="true" minOccurs="0" />
        <xs:element name="user" type="users" nillable="true" minOccurs="0" />
      </xs:sequence>
   </xs:complexType>
</xs:schema> 
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


