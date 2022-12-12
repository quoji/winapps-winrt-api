---
-api-id: M:Microsoft.Windows.Widgets.Providers.IWidgetProvider.Deactivate(System.String)
-api-type: winrt method
---

# Microsoft.Windows.Widgets.Providers.IWidgetProvider.Deactivate(System.String)

<!--
public void Deactivate (string widgetId);
-->


## -description

Notifies the widget provider that the widget host is no longer actively requesting updated content from the provider.

## -parameters

### -param widgetId

The unique identifier of the widget that is being deactivated. The widget ID value is dynamically generated by the <xref:Microsoft.Windows.Widgets.Providers.WidgetManager>. The widget ID remains the same for a widget from the moment of its creation until the moment the Widget is deleted. The widget ID is a unique value across all widgets and all widget providers.

## -remarks

The <xref:Microsoft.Windows.Widgets.Providers.IWidgetProvider.Activate(Microsoft.Windows.Widgets.Providers.WidgetContext)> method is called to notify the widget provider that the widget host is interested in receiving updated content from the provider. These two methods define a window in which the widget host is most interested in showing the most up-to-date content. Widget providers can send updates to the widget at any time, such as in response to a push notification, but as with any background task, it's important to balance providing up-to-date content with resource concerns like battery life. 

## -see-also

## -examples

