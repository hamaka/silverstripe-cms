--- xx-xx-xx			<file path> -	<Customization explanation> ----------------------------------------------


--- 15-4-2015		cms/code/search/SearchForm.php
ipv
		$keywords = $data['Search'];

		hebben we daar nu dit van gemaakt:

		if(isset($data['Search']))
		{
			$keywords = $data['Search'];
		}
		else
		{
			$keywords = '';
		}

		De reden is dat we dan geen error krijgen als je de searchform url rechtstreeks aanroept zonder Search in $_REQUEST


