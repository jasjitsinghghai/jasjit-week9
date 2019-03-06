<?xml version='1.0' encoding='UTF-8' ?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml"
      xmlns:h="http://xmlns.jcp.org/jsf/html"
      xmlns:f="http://java.sun.com/jsf/core"
      xmlns:ui="http://java.sun.com/jsf/facelets">
    <h:head>
        <title>Peter's Facelet Project</title>
    </h:head>
    <h:body>
        
        <h:form>
            <h:panelGrid columns="3">
            <h:outputLabel value="Username" for="username" />
            <h:inputText id="username" required="true" requiredMessage="#{msg['username.validation']}" />
            <h:message for="username" />
            
            <f:facet name="footer">
                <h:commandButton value = "Press This Button" action="/pages/home"/>
            </f:facet>
            </h:panelGrid>

        </h:form>
        
    </h:body>
</html>

<?xml version='1.0' encoding='UTF-8' ?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml"
      xmlns:h="http://xmlns.jcp.org/jsf/html">
    <h:head>
        <title>Facelet Title</title>
    </h:head>
    <h:body>
        Hello from Facelets
    </h:body>
</html>

<?xml version='1.0' encoding='UTF-8'?>
<faces-config version="2.2"
              xmlns="http://xmlns.jcp.org/xml/ns/javaee"
              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
              xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-facesconfig_2_2.xsd">

    <appplication>
        
        <resource-bundle>
            <base-name>com.FirstApp.props</base-name>
            <var>msg</var>
        </resource-bundle>
    </appplication>
</faces-config>
