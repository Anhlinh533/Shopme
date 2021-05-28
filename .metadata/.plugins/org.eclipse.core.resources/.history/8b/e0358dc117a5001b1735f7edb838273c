package com.shopme.admin.user;

import static org.assertj.core.api.Assertions.assertThat;

import org.junit.jupiter.api.Test;
import org.springframework.security.crypto.bcrypt.BCryptPasswordEncoder;

public class PasswordEncodedTest {
	@Test
	public void testEncodedPassword() {
		BCryptPasswordEncoder passEncoder = new BCryptPasswordEncoder();
		String rawPass = "nam2021";
		String encodedPass = passEncoder.encode(rawPass);
		System.out.println(encodedPass);
		boolean matches = passEncoder.matches(rawPass, encodedPass);
		assertThat(matches).isTrue();
	}
}
