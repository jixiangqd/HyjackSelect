###Hyjack Paging###
**Demo Available @ http://hyjack.frontensemble.com** 
<br/>
**Questions, comments, improvements are all welcome!**
<br/>		
<br/>
### Summary ###
*************************************************************************************
  
  Hyjack Select was designed to replace traditional html select input controls (also known

  as combobox or dropdownlists).  Hyjack Select enchances the select by injecting a 

  "search like suggest" textbox which queries the page-loaded select option items.

  The end result is similar to the html5 "datalist" (http://updates.html5rocks.com/2012/04/datalist-landed-in-Chrome-Canary)
<br/>
<br/>
### Remarks ###
*************************************************************************************
  
  The target select control is hidden from the page and replaced by the new 

  "hyjack select" control which is appended using the before() jQuery function.
 
  Any on change event or select value change to the hyjacked control is 

  triggered back to the target select control preventing code breaks on form submit.

  Any modification to display needs to be handled through CSS not hardcoded, sample

  CSS has been embedded in the plugin for reference.
<br/>
<br/>
### Code Samples ###

  <script type='text/javascript'>
    

    /// Single ID which assumes all default 
    
    $('#selector').hyjack_select();


    /// Multiple CLASS with customization 
    
    $('.selector').hyjack_select({          /* Defaults */

        ddImage: 'image/of/arrow.png',      // arrow_down.png

        ddCancel: 'image/of/cancel.png',    // cancel.png

        ddImageClass: 'class_of_arrow',     // hjsel_ddImage

        ddCancelClass: 'class_of_cancel',   // hjsel_ddCancel

        emptyMessage: 'No Items Message',   // No Items to Display

        offset: (int)extra_space,           // 15

        filter: 'search_algorithm',         // 'like', 'first', 'words'

        restrictSearch: false/true          // false

    });
	</script>
	
<br/>
<br/>
### Additional Functions ###
*************************************************************************************	
Often it becomes neccessary to update dropdowns or even disable or dispose of them.

The following is a sub-set of functional available.

	<script type='text/javascript'>

		/// Update Functions
	 
		$.hyjack_select.update('.selector');    // Update by Selector
	 
		$.hyjack_select.update();               // Update All hyjacks


		/// Dispose Functions

		$.hyjack_select.dispose('.selector');   // Dispose by Selector

		$.hyjack_select.dispose();              // Dispose All hyjacks


	</script>
 


*More Examples: http://hyjack.frontensemble.com/*

