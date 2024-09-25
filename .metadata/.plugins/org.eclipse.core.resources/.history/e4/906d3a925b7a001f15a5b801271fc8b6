package com.microservice.Controller;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;
import org.springframework.web.client.RestTemplate;

@RestController
public class UsersController {
	
	@Autowired
	RestTemplate restTemplate;
	
	@GetMapping("/")
	public String getProducts() {
		
		String response =  restTemplate.getForObject("http://MICROSERVICETWO/product", String.class);
		
		
		return response;
	}
}
