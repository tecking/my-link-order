=== My Link Order ===
Contributors: froman118
Donate link: http://geekyweekly.com/mylinkorder
Tags: link, category, categories, order, sidebar, widget
Requires at least: 2.3.2
Tested up to: 2.5.1
Stable tag: 2.5.1

My Link Order allows you to set the order in which links and link categories will appear in the sidebar.

== Description ==

My Link Order allows you to set the order in which links and link categories will appear in the sidebar. Uses a drag 
and drop interface for ordering. Adds a widget with additional options for easy installation on widgetized themes.


== Installation ==

1. Move mylinkorder.php to /wp-content/plugins/
2. Move taxonomy.php to /wp-includes/
3. Activate the My Link Order plugin on the Plugins menu
4. Go to the "My Link Order" tab under Manage and specify your desired order for link categories and links in each category
   
5. If you are using widgets then replace the standard "Links" widget with the "My Link Order" widget. That's it.

6. If you aren't using widgets, modify sidebar template to use correct filter(additional parameter seperated by ampersands):
	wp_list_bookmarks('orderby=order&category_orderby=order'); 


== Frequently Asked Questions ==

= Why modify a core file? =

The way link categories can be ordered is hardcoded at a very low level. Adding an ordering option at that level
makes it easy for people to modify their themes and helps overall compatibility. It also makes my life easier 
since I don't have to duplicate lots of core functions in my plugin just to add a case to one select block.