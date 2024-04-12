# Comparing `tmp/authentik_client-2024.2.2.post1712833897.tar.gz` & `tmp/authentik_client-2024.2.2.post1712922614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.2.2.post1712833897.tar", max compression
+gzip compressed data, was "authentik_client-2024.2.2.post1712922614.tar", max compression
```

## Comparing `authentik_client-2024.2.2.post1712833897.tar` & `authentik_client-2024.2.2.post1712922614.tar`

### file list

```diff
@@ -1,583 +1,583 @@
--rw-r--r--   0        0        0   140605 2024-04-11 11:11:50.688883 authentik_client-2024.2.2.post1712833897/README.md
--rw-r--r--   0        0        0    47475 2024-04-11 11:11:50.700883 authentik_client-2024.2.2.post1712833897/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-11 11:11:50.704883 authentik_client-2024.2.2.post1712833897/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-04-11 11:11:50.360883 authentik_client-2024.2.2.post1712833897/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-04-11 11:11:50.380883 authentik_client-2024.2.2.post1712833897/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   699928 2024-04-11 11:11:50.404883 authentik_client-2024.2.2.post1712833897/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-04-11 11:11:50.416883 authentik_client-2024.2.2.post1712833897/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-04-11 11:11:50.424883 authentik_client-2024.2.2.post1712833897/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-04-11 11:11:50.436883 authentik_client-2024.2.2.post1712833897/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-04-11 11:11:50.452883 authentik_client-2024.2.2.post1712833897/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-04-11 11:11:50.460883 authentik_client-2024.2.2.post1712833897/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-04-11 11:11:50.468883 authentik_client-2024.2.2.post1712833897/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-04-11 11:11:50.488883 authentik_client-2024.2.2.post1712833897/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-04-11 11:11:50.512883 authentik_client-2024.2.2.post1712833897/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   552586 2024-04-11 11:11:50.532883 authentik_client-2024.2.2.post1712833897/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0   718066 2024-04-11 11:11:50.552883 authentik_client-2024.2.2.post1712833897/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-04-11 11:11:50.568883 authentik_client-2024.2.2.post1712833897/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-04-11 11:11:50.580883 authentik_client-2024.2.2.post1712833897/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-04-11 11:11:50.584883 authentik_client-2024.2.2.post1712833897/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-04-11 11:11:50.592883 authentik_client-2024.2.2.post1712833897/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0   802117 2024-04-11 11:11:50.612883 authentik_client-2024.2.2.post1712833897/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945986 2024-04-11 11:11:50.656883 authentik_client-2024.2.2.post1712833897/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-04-11 11:11:50.680883 authentik_client-2024.2.2.post1712833897/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-04-11 11:11:50.708883 authentik_client-2024.2.2.post1712833897/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-04-11 11:11:50.708883 authentik_client-2024.2.2.post1712833897/authentik_client/api_response.py
--rw-r--r--   0        0        0    15345 2024-04-11 11:11:50.700883 authentik_client-2024.2.2.post1712833897/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-04-11 11:11:50.704883 authentik_client-2024.2.2.post1712833897/authentik_client/exceptions.py
--rw-r--r--   0        0        0    45777 2024-04-11 11:11:50.704883 authentik_client-2024.2.2.post1712833897/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-11 11:11:47.376882 authentik_client-2024.2.2.post1712833897/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0     2482 2024-04-11 11:11:47.388882 authentik_client-2024.2.2.post1712833897/authentik_client/models/app.py
--rw-r--r--   0        0        0     4168 2024-04-11 11:11:47.396882 authentik_client-2024.2.2.post1712833897/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-04-11 11:11:47.404882 authentik_client-2024.2.2.post1712833897/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-04-11 11:11:47.416882 authentik_client-2024.2.2.post1712833897/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-04-11 11:11:47.428882 authentik_client-2024.2.2.post1712833897/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-04-11 11:11:47.436882 authentik_client-2024.2.2.post1712833897/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-04-11 11:11:47.444882 authentik_client-2024.2.2.post1712833897/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-04-11 11:11:47.448882 authentik_client-2024.2.2.post1712833897/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     5195 2024-04-11 11:11:47.456882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-04-11 11:11:47.464882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-04-11 11:11:47.472882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-04-11 11:11:47.480882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-04-11 11:11:47.488882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-04-11 11:11:47.492882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-04-11 11:11:47.500882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-04-11 11:11:47.504882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-04-11 11:11:47.504882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-04-11 11:11:47.512882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-04-11 11:11:47.516882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-04-11 11:11:47.524882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-04-11 11:11:47.528882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-04-11 11:11:47.540882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-04-11 11:11:47.544882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-11 11:11:47.552882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-04-11 11:11:47.556882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-04-11 11:11:47.560882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-04-11 11:11:47.568882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-04-11 11:11:47.572882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-04-11 11:11:47.576882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-04-11 11:11:47.584882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-04-11 11:11:47.588882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-04-11 11:11:47.592882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-04-11 11:11:47.596882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-04-11 11:11:47.600882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-04-11 11:11:47.608882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     6722 2024-04-11 11:11:47.612882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4893 2024-04-11 11:11:47.620882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-04-11 11:11:47.624882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-04-11 11:11:47.628882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-04-11 11:11:47.632882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-04-11 11:11:47.636882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-04-11 11:11:47.644882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-04-11 11:11:47.648882 authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-04-11 11:11:47.652882 authentik_client-2024.2.2.post1712833897/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-04-11 11:11:47.660882 authentik_client-2024.2.2.post1712833897/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-04-11 11:11:47.664882 authentik_client-2024.2.2.post1712833897/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-04-11 11:11:47.668882 authentik_client-2024.2.2.post1712833897/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-04-11 11:11:47.672882 authentik_client-2024.2.2.post1712833897/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-04-11 11:11:47.676882 authentik_client-2024.2.2.post1712833897/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-04-11 11:11:47.680882 authentik_client-2024.2.2.post1712833897/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-04-11 11:11:47.684882 authentik_client-2024.2.2.post1712833897/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-04-11 11:11:47.688882 authentik_client-2024.2.2.post1712833897/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-04-11 11:11:47.692882 authentik_client-2024.2.2.post1712833897/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-04-11 11:11:47.696882 authentik_client-2024.2.2.post1712833897/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-04-11 11:11:47.700882 authentik_client-2024.2.2.post1712833897/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-04-11 11:11:47.704882 authentik_client-2024.2.2.post1712833897/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-04-11 11:11:47.708882 authentik_client-2024.2.2.post1712833897/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-04-11 11:11:47.712882 authentik_client-2024.2.2.post1712833897/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-04-11 11:11:47.716882 authentik_client-2024.2.2.post1712833897/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-04-11 11:11:47.720882 authentik_client-2024.2.2.post1712833897/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2861 2024-04-11 11:11:47.724882 authentik_client-2024.2.2.post1712833897/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-04-11 11:11:47.728882 authentik_client-2024.2.2.post1712833897/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-04-11 11:11:47.732882 authentik_client-2024.2.2.post1712833897/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-04-11 11:11:47.736882 authentik_client-2024.2.2.post1712833897/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-04-11 11:11:47.744882 authentik_client-2024.2.2.post1712833897/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-04-11 11:11:47.748882 authentik_client-2024.2.2.post1712833897/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-04-11 11:11:47.752882 authentik_client-2024.2.2.post1712833897/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-04-11 11:11:47.756882 authentik_client-2024.2.2.post1712833897/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-04-11 11:11:47.760882 authentik_client-2024.2.2.post1712833897/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-04-11 11:11:47.768882 authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-04-11 11:11:47.772882 authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-04-11 11:11:47.776882 authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-04-11 11:11:47.780882 authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-04-11 11:11:47.784882 authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-04-11 11:11:47.788882 authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-04-11 11:11:47.792882 authentik_client-2024.2.2.post1712833897/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-04-11 11:11:47.796882 authentik_client-2024.2.2.post1712833897/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-04-11 11:11:47.800882 authentik_client-2024.2.2.post1712833897/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-04-11 11:11:47.808882 authentik_client-2024.2.2.post1712833897/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-04-11 11:11:47.808882 authentik_client-2024.2.2.post1712833897/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-04-11 11:11:47.812882 authentik_client-2024.2.2.post1712833897/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-04-11 11:11:47.820882 authentik_client-2024.2.2.post1712833897/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-04-11 11:11:47.824882 authentik_client-2024.2.2.post1712833897/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-04-11 11:11:47.828882 authentik_client-2024.2.2.post1712833897/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-04-11 11:11:47.832882 authentik_client-2024.2.2.post1712833897/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-04-11 11:11:47.836882 authentik_client-2024.2.2.post1712833897/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-04-11 11:11:47.840882 authentik_client-2024.2.2.post1712833897/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-04-11 11:11:47.840882 authentik_client-2024.2.2.post1712833897/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-04-11 11:11:47.844882 authentik_client-2024.2.2.post1712833897/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-04-11 11:11:47.848882 authentik_client-2024.2.2.post1712833897/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-04-11 11:11:47.852882 authentik_client-2024.2.2.post1712833897/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-04-11 11:11:47.860882 authentik_client-2024.2.2.post1712833897/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-04-11 11:11:47.864882 authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-04-11 11:11:47.868882 authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-04-11 11:11:47.872882 authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-04-11 11:11:47.876882 authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-04-11 11:11:47.880882 authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-04-11 11:11:47.884882 authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-04-11 11:11:47.888882 authentik_client-2024.2.2.post1712833897/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-04-11 11:11:47.892882 authentik_client-2024.2.2.post1712833897/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-04-11 11:11:47.896882 authentik_client-2024.2.2.post1712833897/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-04-11 11:11:47.900882 authentik_client-2024.2.2.post1712833897/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-04-11 11:11:47.904882 authentik_client-2024.2.2.post1712833897/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-04-11 11:11:47.908882 authentik_client-2024.2.2.post1712833897/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-04-11 11:11:47.912882 authentik_client-2024.2.2.post1712833897/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-04-11 11:11:47.920882 authentik_client-2024.2.2.post1712833897/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-04-11 11:11:47.924882 authentik_client-2024.2.2.post1712833897/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-04-11 11:11:47.928882 authentik_client-2024.2.2.post1712833897/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-04-11 11:11:47.936882 authentik_client-2024.2.2.post1712833897/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-04-11 11:11:47.940882 authentik_client-2024.2.2.post1712833897/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-04-11 11:11:47.944882 authentik_client-2024.2.2.post1712833897/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-04-11 11:11:47.948882 authentik_client-2024.2.2.post1712833897/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-04-11 11:11:47.952882 authentik_client-2024.2.2.post1712833897/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-04-11 11:11:47.956882 authentik_client-2024.2.2.post1712833897/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-04-11 11:11:47.960882 authentik_client-2024.2.2.post1712833897/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-04-11 11:11:47.964882 authentik_client-2024.2.2.post1712833897/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3926 2024-04-11 11:11:47.968882 authentik_client-2024.2.2.post1712833897/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-04-11 11:11:47.972882 authentik_client-2024.2.2.post1712833897/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-04-11 11:11:47.976882 authentik_client-2024.2.2.post1712833897/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-04-11 11:11:47.984882 authentik_client-2024.2.2.post1712833897/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-04-11 11:11:47.988882 authentik_client-2024.2.2.post1712833897/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-04-11 11:11:47.992882 authentik_client-2024.2.2.post1712833897/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-04-11 11:11:47.996882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-04-11 11:11:48.004882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-04-11 11:11:48.004882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-04-11 11:11:48.008882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-04-11 11:11:48.016882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-04-11 11:11:48.020882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-04-11 11:11:48.024882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-04-11 11:11:48.028882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-04-11 11:11:48.032882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-04-11 11:11:48.036882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-04-11 11:11:48.040882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-04-11 11:11:48.048882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-04-11 11:11:48.052882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-04-11 11:11:48.060882 authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-04-11 11:11:48.060882 authentik_client-2024.2.2.post1712833897/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-04-11 11:11:48.064882 authentik_client-2024.2.2.post1712833897/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-04-11 11:11:48.068882 authentik_client-2024.2.2.post1712833897/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     5216 2024-04-11 11:11:48.072882 authentik_client-2024.2.2.post1712833897/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-04-11 11:11:48.076882 authentik_client-2024.2.2.post1712833897/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-04-11 11:11:48.080882 authentik_client-2024.2.2.post1712833897/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-04-11 11:11:48.084882 authentik_client-2024.2.2.post1712833897/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-04-11 11:11:48.088882 authentik_client-2024.2.2.post1712833897/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-04-11 11:11:48.092882 authentik_client-2024.2.2.post1712833897/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-04-11 11:11:48.096882 authentik_client-2024.2.2.post1712833897/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-04-11 11:11:48.100882 authentik_client-2024.2.2.post1712833897/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-04-11 11:11:48.104882 authentik_client-2024.2.2.post1712833897/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-04-11 11:11:48.108882 authentik_client-2024.2.2.post1712833897/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-04-11 11:11:48.108882 authentik_client-2024.2.2.post1712833897/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4878 2024-04-11 11:11:48.112882 authentik_client-2024.2.2.post1712833897/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3895 2024-04-11 11:11:48.120882 authentik_client-2024.2.2.post1712833897/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-04-11 11:11:48.124882 authentik_client-2024.2.2.post1712833897/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-04-11 11:11:48.128882 authentik_client-2024.2.2.post1712833897/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-04-11 11:11:48.132882 authentik_client-2024.2.2.post1712833897/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-04-11 11:11:48.136882 authentik_client-2024.2.2.post1712833897/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-04-11 11:11:48.140882 authentik_client-2024.2.2.post1712833897/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-04-11 11:11:48.144882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-04-11 11:11:48.152882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-04-11 11:11:48.156882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-04-11 11:11:48.160882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-04-11 11:11:48.164882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-04-11 11:11:48.168882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-04-11 11:11:48.176882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-04-11 11:11:48.180882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0     3129 2024-04-11 11:11:48.188882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_sync_status.py
--rw-r--r--   0        0        0      726 2024-04-11 11:11:48.140882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-04-11 11:11:48.192882 authentik_client-2024.2.2.post1712833897/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-04-11 11:11:48.196882 authentik_client-2024.2.2.post1712833897/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-04-11 11:11:48.200882 authentik_client-2024.2.2.post1712833897/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-04-11 11:11:48.204882 authentik_client-2024.2.2.post1712833897/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-04-11 11:11:48.208882 authentik_client-2024.2.2.post1712833897/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-04-11 11:11:48.216882 authentik_client-2024.2.2.post1712833897/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-04-11 11:11:48.216882 authentik_client-2024.2.2.post1712833897/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-04-11 11:11:48.220882 authentik_client-2024.2.2.post1712833897/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-04-11 11:11:48.224882 authentik_client-2024.2.2.post1712833897/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-04-11 11:11:48.228882 authentik_client-2024.2.2.post1712833897/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-04-11 11:11:48.232882 authentik_client-2024.2.2.post1712833897/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     7524 2024-04-11 11:11:48.232882 authentik_client-2024.2.2.post1712833897/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0     9828 2024-04-11 11:11:48.236882 authentik_client-2024.2.2.post1712833897/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-04-11 11:11:48.240882 authentik_client-2024.2.2.post1712833897/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-04-11 11:11:48.240882 authentik_client-2024.2.2.post1712833897/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-04-11 11:11:48.244882 authentik_client-2024.2.2.post1712833897/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-04-11 11:11:48.248882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-04-11 11:11:48.248882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-04-11 11:11:48.252882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-04-11 11:11:48.256882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-04-11 11:11:48.260882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-04-11 11:11:48.264882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-04-11 11:11:48.268882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-04-11 11:11:48.272882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-04-11 11:11:48.272882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-04-11 11:11:48.276882 authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-04-11 11:11:48.280882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-04-11 11:11:48.284882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-04-11 11:11:48.288882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-04-11 11:11:48.292882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-04-11 11:11:48.296882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-04-11 11:11:48.300882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-04-11 11:11:48.304882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-04-11 11:11:48.308882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8013 2024-04-11 11:11:48.312882 authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-04-11 11:11:48.316882 authentik_client-2024.2.2.post1712833897/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0     5545 2024-04-11 11:11:48.324882 authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-04-11 11:11:48.324882 authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-04-11 11:11:48.328882 authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-04-11 11:11:48.332882 authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-04-11 11:11:48.336882 authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-04-11 11:11:48.340882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-04-11 11:11:48.344882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-04-11 11:11:48.348882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-04-11 11:11:48.348882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-04-11 11:11:48.352882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-04-11 11:11:48.356882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-04-11 11:11:48.360882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-04-11 11:11:48.364882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-04-11 11:11:48.368882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-04-11 11:11:48.372882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-04-11 11:11:48.376882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-04-11 11:11:48.380882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-04-11 11:11:48.384882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-04-11 11:11:48.388882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-11 11:11:48.392882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-04-11 11:11:48.396882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-04-11 11:11:48.400882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-04-11 11:11:48.404882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-04-11 11:11:48.412882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-11 11:11:48.416882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-11 11:11:48.420882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-04-11 11:11:48.424882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-04-11 11:11:48.428882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-04-11 11:11:48.432882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-04-11 11:11:48.440882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-04-11 11:11:48.444882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-04-11 11:11:48.448882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-04-11 11:11:48.448882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-11 11:11:48.452882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-04-11 11:11:48.456882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3274 2024-04-11 11:11:48.460882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-04-11 11:11:48.464882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-11 11:11:48.468882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-04-11 11:11:48.472882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-04-11 11:11:48.476882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-04-11 11:11:48.480882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-04-11 11:11:48.484882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-11 11:11:48.484882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-11 11:11:48.488882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-11 11:11:48.492882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3330 2024-04-11 11:11:48.496882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-04-11 11:11:48.500882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-04-11 11:11:48.504882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-04-11 11:11:48.508882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-04-11 11:11:48.512882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-04-11 11:11:48.512882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-11 11:11:48.520882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-04-11 11:11:48.524882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-04-11 11:11:48.528882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-04-11 11:11:48.532882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-11 11:11:48.536882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-04-11 11:11:48.540882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-04-11 11:11:48.544882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-04-11 11:11:48.548882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-04-11 11:11:48.552882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-04-11 11:11:48.556882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-04-11 11:11:48.560882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-04-11 11:11:48.564882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-04-11 11:11:48.568882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-11 11:11:48.568882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-04-11 11:11:48.572882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-11 11:11:48.576882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-04-11 11:11:48.580882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-04-11 11:11:48.584882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-04-11 11:11:48.588882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-04-11 11:11:48.592882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-04-11 11:11:48.596882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-04-11 11:11:48.596882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-11 11:11:48.600882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-04-11 11:11:48.604882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-11 11:11:48.608882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-11 11:11:48.612882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-11 11:11:48.612882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-11 11:11:48.616882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3331 2024-04-11 11:11:48.624882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-04-11 11:11:48.628882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-04-11 11:11:48.620882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-04-11 11:11:48.632882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-11 11:11:48.632882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-04-11 11:11:48.636882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-04-11 11:11:48.640882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-11 11:11:48.644882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-04-11 11:11:48.648882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-04-11 11:11:48.652882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-04-11 11:11:48.656882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-04-11 11:11:48.644882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-04-11 11:11:48.660882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-04-11 11:11:48.664882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-04-11 11:11:48.664882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-04-11 11:11:48.668882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-04-11 11:11:48.672882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-04-11 11:11:48.676882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-04-11 11:11:48.680882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-04-11 11:11:48.680882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-04-11 11:11:48.684882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-04-11 11:11:48.688882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-04-11 11:11:48.692882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-04-11 11:11:48.696882 authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-04-11 11:11:48.696882 authentik_client-2024.2.2.post1712833897/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-04-11 11:11:48.700882 authentik_client-2024.2.2.post1712833897/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-04-11 11:11:48.704882 authentik_client-2024.2.2.post1712833897/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-04-11 11:11:48.708882 authentik_client-2024.2.2.post1712833897/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-04-11 11:11:48.712882 authentik_client-2024.2.2.post1712833897/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-04-11 11:11:48.712882 authentik_client-2024.2.2.post1712833897/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-04-11 11:11:48.716882 authentik_client-2024.2.2.post1712833897/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-04-11 11:11:48.720882 authentik_client-2024.2.2.post1712833897/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-04-11 11:11:48.728882 authentik_client-2024.2.2.post1712833897/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-11 11:11:48.732882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-04-11 11:11:48.732882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-04-11 11:11:48.736882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-04-11 11:11:48.740882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-04-11 11:11:48.744882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4931 2024-04-11 11:11:48.748882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-04-11 11:11:48.752882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-04-11 11:11:48.756882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-04-11 11:11:48.760882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-04-11 11:11:48.764882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-04-11 11:11:48.764882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-04-11 11:11:48.768882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-04-11 11:11:48.772882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-04-11 11:11:48.776882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-04-11 11:11:48.780882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-04-11 11:11:48.784882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-04-11 11:11:48.788882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-04-11 11:11:48.792882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-04-11 11:11:48.792882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-04-11 11:11:48.796882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-04-11 11:11:48.800882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-04-11 11:11:48.804882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-04-11 11:11:48.808882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-04-11 11:11:48.812882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-04-11 11:11:48.816882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-04-11 11:11:48.820882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     3385 2024-04-11 11:11:48.824882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-04-11 11:11:48.828882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3985 2024-04-11 11:11:48.832882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-04-11 11:11:48.836882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-04-11 11:11:48.840882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-04-11 11:11:48.844882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-04-11 11:11:48.848882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-04-11 11:11:48.852882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-04-11 11:11:48.856882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2879 2024-04-11 11:11:48.860882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-04-11 11:11:48.864882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-04-11 11:11:48.868882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-04-11 11:11:48.872882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-04-11 11:11:48.876882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8185 2024-04-11 11:11:48.880882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-04-11 11:11:48.884882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-04-11 11:11:48.888882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-04-11 11:11:48.892882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-04-11 11:11:48.896882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-04-11 11:11:48.900882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-04-11 11:11:48.904882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-04-11 11:11:48.908882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-04-11 11:11:48.916882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-04-11 11:11:48.920882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-04-11 11:11:48.924882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-04-11 11:11:48.928882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-04-11 11:11:48.932882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-04-11 11:11:48.932882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-04-11 11:11:48.936882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-04-11 11:11:48.940882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-04-11 11:11:48.944882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-04-11 11:11:48.944882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-04-11 11:11:48.948882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-04-11 11:11:48.952882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-04-11 11:11:48.956882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-04-11 11:11:48.960882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3819 2024-04-11 11:11:48.964882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     5079 2024-04-11 11:11:48.968882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-04-11 11:11:48.964882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-04-11 11:11:48.972882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-04-11 11:11:48.976882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-04-11 11:11:48.984882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4419 2024-04-11 11:11:48.988882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-04-11 11:11:48.980882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-04-11 11:11:48.992882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-04-11 11:11:48.996882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-04-11 11:11:49.000882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-04-11 11:11:49.000882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-04-11 11:11:49.004882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-04-11 11:11:49.008882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-04-11 11:11:49.008882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-04-11 11:11:49.012882 authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-04-11 11:11:49.016882 authentik_client-2024.2.2.post1712833897/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-04-11 11:11:49.020882 authentik_client-2024.2.2.post1712833897/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-04-11 11:11:49.024882 authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-04-11 11:11:49.024882 authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-04-11 11:11:49.028882 authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-04-11 11:11:49.032882 authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-04-11 11:11:49.036882 authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-04-11 11:11:49.040882 authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-04-11 11:11:49.040882 authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-04-11 11:11:49.044882 authentik_client-2024.2.2.post1712833897/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-04-11 11:11:49.048882 authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-04-11 11:11:49.052882 authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-04-11 11:11:49.052882 authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-04-11 11:11:49.060882 authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-04-11 11:11:49.060882 authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-04-11 11:11:49.068882 authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-04-11 11:11:49.072882 authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-04-11 11:11:49.076882 authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-04-11 11:11:49.076882 authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-04-11 11:11:49.080882 authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-04-11 11:11:49.084882 authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-04-11 11:11:49.088882 authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-04-11 11:11:49.092882 authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-04-11 11:11:49.096882 authentik_client-2024.2.2.post1712833897/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-04-11 11:11:49.100882 authentik_client-2024.2.2.post1712833897/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-04-11 11:11:49.100882 authentik_client-2024.2.2.post1712833897/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-04-11 11:11:49.104882 authentik_client-2024.2.2.post1712833897/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-04-11 11:11:49.108882 authentik_client-2024.2.2.post1712833897/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-04-11 11:11:49.108882 authentik_client-2024.2.2.post1712833897/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1314 2024-04-11 11:11:49.112882 authentik_client-2024.2.2.post1712833897/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-04-11 11:11:49.112882 authentik_client-2024.2.2.post1712833897/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-04-11 11:11:49.116882 authentik_client-2024.2.2.post1712833897/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-04-11 11:11:49.116882 authentik_client-2024.2.2.post1712833897/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-04-11 11:11:49.120882 authentik_client-2024.2.2.post1712833897/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-04-11 11:11:49.124882 authentik_client-2024.2.2.post1712833897/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-04-11 11:11:49.128882 authentik_client-2024.2.2.post1712833897/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-04-11 11:11:49.132882 authentik_client-2024.2.2.post1712833897/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-04-11 11:11:49.132882 authentik_client-2024.2.2.post1712833897/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-04-11 11:11:49.136882 authentik_client-2024.2.2.post1712833897/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-04-11 11:11:49.140882 authentik_client-2024.2.2.post1712833897/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-04-11 11:11:49.144882 authentik_client-2024.2.2.post1712833897/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-04-11 11:11:49.144882 authentik_client-2024.2.2.post1712833897/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-04-11 11:11:49.148882 authentik_client-2024.2.2.post1712833897/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-04-11 11:11:49.152882 authentik_client-2024.2.2.post1712833897/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-04-11 11:11:49.152882 authentik_client-2024.2.2.post1712833897/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-04-11 11:11:49.156882 authentik_client-2024.2.2.post1712833897/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-04-11 11:11:49.160882 authentik_client-2024.2.2.post1712833897/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-04-11 11:11:49.160882 authentik_client-2024.2.2.post1712833897/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-04-11 11:11:49.164882 authentik_client-2024.2.2.post1712833897/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-04-11 11:11:49.168882 authentik_client-2024.2.2.post1712833897/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-04-11 11:11:49.172882 authentik_client-2024.2.2.post1712833897/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-04-11 11:11:49.172882 authentik_client-2024.2.2.post1712833897/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-04-11 11:11:49.176882 authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-04-11 11:11:49.180882 authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-04-11 11:11:49.184882 authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-04-11 11:11:49.188882 authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-04-11 11:11:49.188882 authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-04-11 11:11:49.192882 authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-04-11 11:11:49.196882 authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-04-11 11:11:49.200882 authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-04-11 11:11:49.204882 authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-04-11 11:11:49.208882 authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-04-11 11:11:49.212882 authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     3131 2024-04-11 11:11:49.216882 authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_sync_status.py
--rw-r--r--   0        0        0     4629 2024-04-11 11:11:49.224882 authentik_client-2024.2.2.post1712833897/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-04-11 11:11:49.228882 authentik_client-2024.2.2.post1712833897/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-04-11 11:11:49.228882 authentik_client-2024.2.2.post1712833897/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-04-11 11:11:49.232882 authentik_client-2024.2.2.post1712833897/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-04-11 11:11:49.236882 authentik_client-2024.2.2.post1712833897/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-04-11 11:11:49.240882 authentik_client-2024.2.2.post1712833897/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-04-11 11:11:49.244882 authentik_client-2024.2.2.post1712833897/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4931 2024-04-11 11:11:49.244882 authentik_client-2024.2.2.post1712833897/authentik_client/models/settings.py
--rw-r--r--   0        0        0     5058 2024-04-11 11:11:49.248882 authentik_client-2024.2.2.post1712833897/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-04-11 11:11:49.252882 authentik_client-2024.2.2.post1712833897/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-04-11 11:11:49.252882 authentik_client-2024.2.2.post1712833897/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     1492 2024-04-11 11:11:49.256882 authentik_client-2024.2.2.post1712833897/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-04-11 11:11:49.220882 authentik_client-2024.2.2.post1712833897/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-04-11 11:11:49.220882 authentik_client-2024.2.2.post1712833897/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-04-11 11:11:49.260882 authentik_client-2024.2.2.post1712833897/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-04-11 11:11:49.264882 authentik_client-2024.2.2.post1712833897/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-04-11 11:11:49.268882 authentik_client-2024.2.2.post1712833897/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-04-11 11:11:49.272882 authentik_client-2024.2.2.post1712833897/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-04-11 11:11:49.276882 authentik_client-2024.2.2.post1712833897/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-04-11 11:11:49.276882 authentik_client-2024.2.2.post1712833897/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-04-11 11:11:49.280882 authentik_client-2024.2.2.post1712833897/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-04-11 11:11:49.284882 authentik_client-2024.2.2.post1712833897/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-04-11 11:11:49.288882 authentik_client-2024.2.2.post1712833897/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-04-11 11:11:49.292882 authentik_client-2024.2.2.post1712833897/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-04-11 11:11:49.296882 authentik_client-2024.2.2.post1712833897/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-04-11 11:11:49.300882 authentik_client-2024.2.2.post1712833897/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-04-11 11:11:49.304882 authentik_client-2024.2.2.post1712833897/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-04-11 11:11:49.304882 authentik_client-2024.2.2.post1712833897/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     4463 2024-04-11 11:11:49.308882 authentik_client-2024.2.2.post1712833897/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-04-11 11:11:49.308882 authentik_client-2024.2.2.post1712833897/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4286 2024-04-11 11:11:49.312882 authentik_client-2024.2.2.post1712833897/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-04-11 11:11:49.312882 authentik_client-2024.2.2.post1712833897/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-04-11 11:11:49.320882 authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-04-11 11:11:49.324882 authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-04-11 11:11:49.324882 authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-04-11 11:11:49.328882 authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-04-11 11:11:49.328882 authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4802 2024-04-11 11:11:49.332883 authentik_client-2024.2.2.post1712833897/authentik_client/models/token.py
--rw-r--r--   0        0        0     4198 2024-04-11 11:11:49.336882 authentik_client-2024.2.2.post1712833897/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4329 2024-04-11 11:11:49.336882 authentik_client-2024.2.2.post1712833897/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-04-11 11:11:49.340882 authentik_client-2024.2.2.post1712833897/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-04-11 11:11:49.340882 authentik_client-2024.2.2.post1712833897/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-04-11 11:11:49.316882 authentik_client-2024.2.2.post1712833897/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-04-11 11:11:49.316882 authentik_client-2024.2.2.post1712833897/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-04-11 11:11:49.344882 authentik_client-2024.2.2.post1712833897/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-04-11 11:11:49.348882 authentik_client-2024.2.2.post1712833897/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-04-11 11:11:49.348882 authentik_client-2024.2.2.post1712833897/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-04-11 11:11:49.352882 authentik_client-2024.2.2.post1712833897/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-04-11 11:11:49.352882 authentik_client-2024.2.2.post1712833897/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-04-11 11:11:49.356882 authentik_client-2024.2.2.post1712833897/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5226 2024-04-11 11:11:49.356882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-04-11 11:11:49.360882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-04-11 11:11:49.364882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3828 2024-04-11 11:11:49.364882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-04-11 11:11:49.368883 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-04-11 11:11:49.368883 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-04-11 11:11:49.372882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-04-11 11:11:49.376882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-04-11 11:11:49.380882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     3193 2024-04-11 11:11:49.384882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_group_request.py
--rw-r--r--   0        0        0     4334 2024-04-11 11:11:49.388882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-04-11 11:11:49.392882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-04-11 11:11:49.396882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-04-11 11:11:49.396882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-04-11 11:11:49.400882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-04-11 11:11:49.404883 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-04-11 11:11:49.404883 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-04-11 11:11:49.408882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-04-11 11:11:49.408882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-04-11 11:11:49.412882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-04-11 11:11:49.416882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-04-11 11:11:49.416882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-04-11 11:11:49.420882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-04-11 11:11:49.424883 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-04-11 11:11:49.424883 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-04-11 11:11:49.428882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-04-11 11:11:49.432882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-04-11 11:11:49.436882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-04-11 11:11:49.436882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-04-11 11:11:49.440883 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-04-11 11:11:49.444882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-04-11 11:11:49.448882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-04-11 11:11:49.448882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-04-11 11:11:49.448882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-04-11 11:11:49.452882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-04-11 11:11:49.456882 authentik_client-2024.2.2.post1712833897/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-04-11 11:11:49.460883 authentik_client-2024.2.2.post1712833897/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-04-11 11:11:49.460883 authentik_client-2024.2.2.post1712833897/authentik_client/models/version.py
--rw-r--r--   0        0        0     3630 2024-04-11 11:11:49.464882 authentik_client-2024.2.2.post1712833897/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-04-11 11:11:49.464882 authentik_client-2024.2.2.post1712833897/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-04-11 11:11:49.468882 authentik_client-2024.2.2.post1712833897/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-04-11 11:11:49.468882 authentik_client-2024.2.2.post1712833897/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-04-11 11:11:49.472882 authentik_client-2024.2.2.post1712833897/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-04-11 11:11:50.696883 authentik_client-2024.2.2.post1712833897/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-04-11 11:11:50.708883 authentik_client-2024.2.2.post1712833897/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-04-11 11:11:50.696883 authentik_client-2024.2.2.post1712833897/pyproject.toml
--rw-r--r--   0        0        0   141557 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1712833897/PKG-INFO
+-rw-r--r--   0        0        0   140456 2024-04-12 11:50:27.891247 authentik_client-2024.2.2.post1712922614/README.md
+-rw-r--r--   0        0        0    47475 2024-04-12 11:50:27.903247 authentik_client-2024.2.2.post1712922614/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-12 11:50:27.907247 authentik_client-2024.2.2.post1712922614/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-04-12 11:50:27.627245 authentik_client-2024.2.2.post1712922614/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-04-12 11:50:27.651245 authentik_client-2024.2.2.post1712922614/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   699928 2024-04-12 11:50:27.671245 authentik_client-2024.2.2.post1712922614/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-04-12 11:50:27.683246 authentik_client-2024.2.2.post1712922614/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-04-12 11:50:27.691246 authentik_client-2024.2.2.post1712922614/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-04-12 11:50:27.699246 authentik_client-2024.2.2.post1712922614/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-04-12 11:50:27.711246 authentik_client-2024.2.2.post1712922614/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-04-12 11:50:27.719246 authentik_client-2024.2.2.post1712922614/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-04-12 11:50:27.735246 authentik_client-2024.2.2.post1712922614/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-04-12 11:50:27.747246 authentik_client-2024.2.2.post1712922614/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-04-12 11:50:27.759246 authentik_client-2024.2.2.post1712922614/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   552586 2024-04-12 11:50:27.775246 authentik_client-2024.2.2.post1712922614/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0   718066 2024-04-12 11:50:27.799246 authentik_client-2024.2.2.post1712922614/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-04-12 11:50:27.815246 authentik_client-2024.2.2.post1712922614/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-04-12 11:50:27.823246 authentik_client-2024.2.2.post1712922614/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-04-12 11:50:27.831246 authentik_client-2024.2.2.post1712922614/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-04-12 11:50:27.835246 authentik_client-2024.2.2.post1712922614/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0   802117 2024-04-12 11:50:27.847246 authentik_client-2024.2.2.post1712922614/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-04-12 11:50:27.871246 authentik_client-2024.2.2.post1712922614/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-04-12 11:50:27.883247 authentik_client-2024.2.2.post1712922614/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-04-12 11:50:27.907247 authentik_client-2024.2.2.post1712922614/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-12 11:50:27.911247 authentik_client-2024.2.2.post1712922614/authentik_client/api_response.py
+-rw-r--r--   0        0        0    14724 2024-04-12 11:50:27.903247 authentik_client-2024.2.2.post1712922614/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-04-12 11:50:27.907247 authentik_client-2024.2.2.post1712922614/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    45777 2024-04-12 11:50:27.903247 authentik_client-2024.2.2.post1712922614/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-04-12 11:50:24.575224 authentik_client-2024.2.2.post1712922614/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0     2482 2024-04-12 11:50:24.591224 authentik_client-2024.2.2.post1712922614/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4168 2024-04-12 11:50:24.599224 authentik_client-2024.2.2.post1712922614/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-04-12 11:50:24.615224 authentik_client-2024.2.2.post1712922614/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-04-12 11:50:24.627225 authentik_client-2024.2.2.post1712922614/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-04-12 11:50:24.639225 authentik_client-2024.2.2.post1712922614/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-04-12 11:50:24.651225 authentik_client-2024.2.2.post1712922614/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-04-12 11:50:24.659225 authentik_client-2024.2.2.post1712922614/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-04-12 11:50:24.663225 authentik_client-2024.2.2.post1712922614/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     5195 2024-04-12 11:50:24.671225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-04-12 11:50:24.679225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-04-12 11:50:24.691225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-04-12 11:50:24.699225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-04-12 11:50:24.707225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-04-12 11:50:24.715225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-04-12 11:50:24.727225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-04-12 11:50:24.731226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-04-12 11:50:24.735226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-04-12 11:50:24.747226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-04-12 11:50:24.755226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-04-12 11:50:24.767226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-04-12 11:50:24.775226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-04-12 11:50:24.783226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-04-12 11:50:24.791226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-12 11:50:24.799226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-04-12 11:50:24.807226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-04-12 11:50:24.811226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-04-12 11:50:24.819226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-04-12 11:50:24.827226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-04-12 11:50:24.835226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-04-12 11:50:24.839227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-04-12 11:50:24.843227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-04-12 11:50:24.851227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-04-12 11:50:24.855227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-04-12 11:50:24.859227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-04-12 11:50:24.867227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     6722 2024-04-12 11:50:24.875227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4893 2024-04-12 11:50:24.879227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-04-12 11:50:24.887227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-04-12 11:50:24.895227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-04-12 11:50:24.903227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-04-12 11:50:24.907227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-04-12 11:50:24.911227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-04-12 11:50:24.919227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-04-12 11:50:24.923227 authentik_client-2024.2.2.post1712922614/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-04-12 11:50:24.927227 authentik_client-2024.2.2.post1712922614/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-04-12 11:50:24.931228 authentik_client-2024.2.2.post1712922614/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-04-12 11:50:24.935227 authentik_client-2024.2.2.post1712922614/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-04-12 11:50:24.939227 authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-04-12 11:50:24.947228 authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-04-12 11:50:24.955228 authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-04-12 11:50:24.963228 authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-04-12 11:50:24.967228 authentik_client-2024.2.2.post1712922614/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-04-12 11:50:24.971228 authentik_client-2024.2.2.post1712922614/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-04-12 11:50:24.975228 authentik_client-2024.2.2.post1712922614/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-04-12 11:50:24.979228 authentik_client-2024.2.2.post1712922614/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-04-12 11:50:24.983228 authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-04-12 11:50:24.987228 authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-04-12 11:50:24.991228 authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-04-12 11:50:24.995228 authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-04-12 11:50:24.999228 authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2861 2024-04-12 11:50:25.007228 authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-04-12 11:50:25.011228 authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-04-12 11:50:25.015228 authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-04-12 11:50:25.019228 authentik_client-2024.2.2.post1712922614/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-04-12 11:50:25.027228 authentik_client-2024.2.2.post1712922614/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-04-12 11:50:25.031228 authentik_client-2024.2.2.post1712922614/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-04-12 11:50:25.035229 authentik_client-2024.2.2.post1712922614/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-04-12 11:50:25.039229 authentik_client-2024.2.2.post1712922614/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-04-12 11:50:25.043228 authentik_client-2024.2.2.post1712922614/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-04-12 11:50:25.047229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-04-12 11:50:25.055229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-04-12 11:50:25.063229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-04-12 11:50:25.075229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-04-12 11:50:25.079229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-04-12 11:50:25.083229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-04-12 11:50:25.091229 authentik_client-2024.2.2.post1712922614/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-04-12 11:50:25.095229 authentik_client-2024.2.2.post1712922614/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-04-12 11:50:25.103229 authentik_client-2024.2.2.post1712922614/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-04-12 11:50:25.111229 authentik_client-2024.2.2.post1712922614/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-04-12 11:50:25.115229 authentik_client-2024.2.2.post1712922614/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-04-12 11:50:25.123229 authentik_client-2024.2.2.post1712922614/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-04-12 11:50:25.131229 authentik_client-2024.2.2.post1712922614/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-04-12 11:50:25.139229 authentik_client-2024.2.2.post1712922614/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-04-12 11:50:25.147230 authentik_client-2024.2.2.post1712922614/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-04-12 11:50:25.155230 authentik_client-2024.2.2.post1712922614/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-04-12 11:50:25.159230 authentik_client-2024.2.2.post1712922614/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-04-12 11:50:25.163230 authentik_client-2024.2.2.post1712922614/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-04-12 11:50:25.163230 authentik_client-2024.2.2.post1712922614/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-04-12 11:50:25.171230 authentik_client-2024.2.2.post1712922614/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-04-12 11:50:25.179230 authentik_client-2024.2.2.post1712922614/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-04-12 11:50:25.187230 authentik_client-2024.2.2.post1712922614/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-04-12 11:50:25.199230 authentik_client-2024.2.2.post1712922614/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-04-12 11:50:25.207230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-04-12 11:50:25.215230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-04-12 11:50:25.219230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-04-12 11:50:25.227230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-04-12 11:50:25.235231 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-04-12 11:50:25.243230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-04-12 11:50:25.247231 authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-04-12 11:50:25.255231 authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-04-12 11:50:25.263231 authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-04-12 11:50:25.263231 authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-04-12 11:50:25.271231 authentik_client-2024.2.2.post1712922614/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-04-12 11:50:25.279231 authentik_client-2024.2.2.post1712922614/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-04-12 11:50:25.287231 authentik_client-2024.2.2.post1712922614/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-04-12 11:50:25.295231 authentik_client-2024.2.2.post1712922614/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-04-12 11:50:25.299231 authentik_client-2024.2.2.post1712922614/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-04-12 11:50:25.307231 authentik_client-2024.2.2.post1712922614/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-04-12 11:50:25.315231 authentik_client-2024.2.2.post1712922614/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-04-12 11:50:25.323231 authentik_client-2024.2.2.post1712922614/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-04-12 11:50:25.331231 authentik_client-2024.2.2.post1712922614/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-04-12 11:50:25.335231 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-04-12 11:50:25.339231 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-04-12 11:50:25.347231 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-04-12 11:50:25.351232 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-04-12 11:50:25.359232 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3926 2024-04-12 11:50:25.367232 authentik_client-2024.2.2.post1712922614/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-04-12 11:50:25.375232 authentik_client-2024.2.2.post1712922614/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-04-12 11:50:25.383232 authentik_client-2024.2.2.post1712922614/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-04-12 11:50:25.391232 authentik_client-2024.2.2.post1712922614/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-04-12 11:50:25.395232 authentik_client-2024.2.2.post1712922614/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-04-12 11:50:25.403232 authentik_client-2024.2.2.post1712922614/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-04-12 11:50:25.411232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-04-12 11:50:25.419232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-04-12 11:50:25.423232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-04-12 11:50:25.427232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-04-12 11:50:25.439232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-04-12 11:50:25.443232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-04-12 11:50:25.451233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-04-12 11:50:25.459233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-04-12 11:50:25.463233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-04-12 11:50:25.471233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-04-12 11:50:25.479233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-04-12 11:50:25.483233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-04-12 11:50:25.487233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-04-12 11:50:25.487233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-04-12 11:50:25.491233 authentik_client-2024.2.2.post1712922614/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-04-12 11:50:25.495233 authentik_client-2024.2.2.post1712922614/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-04-12 11:50:25.499233 authentik_client-2024.2.2.post1712922614/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     5216 2024-04-12 11:50:25.499233 authentik_client-2024.2.2.post1712922614/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-04-12 11:50:25.507233 authentik_client-2024.2.2.post1712922614/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-04-12 11:50:25.511233 authentik_client-2024.2.2.post1712922614/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-04-12 11:50:25.515233 authentik_client-2024.2.2.post1712922614/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-04-12 11:50:25.519233 authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-04-12 11:50:25.523233 authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-04-12 11:50:25.527233 authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-04-12 11:50:25.531233 authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-04-12 11:50:25.535233 authentik_client-2024.2.2.post1712922614/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-04-12 11:50:25.535233 authentik_client-2024.2.2.post1712922614/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-04-12 11:50:25.539234 authentik_client-2024.2.2.post1712922614/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4878 2024-04-12 11:50:25.543233 authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3895 2024-04-12 11:50:25.547233 authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-04-12 11:50:25.551234 authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-04-12 11:50:25.555234 authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-04-12 11:50:25.555234 authentik_client-2024.2.2.post1712922614/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-04-12 11:50:25.559234 authentik_client-2024.2.2.post1712922614/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-04-12 11:50:25.563234 authentik_client-2024.2.2.post1712922614/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-04-12 11:50:25.567234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-04-12 11:50:25.571234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-04-12 11:50:25.575234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-04-12 11:50:25.579234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-04-12 11:50:25.583234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-04-12 11:50:25.587234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-04-12 11:50:25.591234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-04-12 11:50:25.595234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0     3129 2024-04-12 11:50:25.599234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_sync_status.py
+-rw-r--r--   0        0        0      726 2024-04-12 11:50:25.563234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-04-12 11:50:25.603234 authentik_client-2024.2.2.post1712922614/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-04-12 11:50:25.607234 authentik_client-2024.2.2.post1712922614/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-04-12 11:50:25.611234 authentik_client-2024.2.2.post1712922614/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-04-12 11:50:25.615234 authentik_client-2024.2.2.post1712922614/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-04-12 11:50:25.619234 authentik_client-2024.2.2.post1712922614/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-04-12 11:50:25.623234 authentik_client-2024.2.2.post1712922614/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-04-12 11:50:25.627234 authentik_client-2024.2.2.post1712922614/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-04-12 11:50:25.631234 authentik_client-2024.2.2.post1712922614/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-04-12 11:50:25.635234 authentik_client-2024.2.2.post1712922614/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-04-12 11:50:25.639234 authentik_client-2024.2.2.post1712922614/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-04-12 11:50:25.643234 authentik_client-2024.2.2.post1712922614/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     7524 2024-04-12 11:50:25.647235 authentik_client-2024.2.2.post1712922614/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0     9828 2024-04-12 11:50:25.651234 authentik_client-2024.2.2.post1712922614/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-04-12 11:50:25.655235 authentik_client-2024.2.2.post1712922614/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-04-12 11:50:25.659235 authentik_client-2024.2.2.post1712922614/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-04-12 11:50:25.663235 authentik_client-2024.2.2.post1712922614/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-04-12 11:50:25.663235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-04-12 11:50:25.671235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-04-12 11:50:25.675235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-04-12 11:50:25.679235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-04-12 11:50:25.683235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-04-12 11:50:25.687235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-04-12 11:50:25.691235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-04-12 11:50:25.695235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-04-12 11:50:25.699235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-04-12 11:50:25.703235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-04-12 11:50:25.707235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-04-12 11:50:25.711235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-04-12 11:50:25.715235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-04-12 11:50:25.719235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-04-12 11:50:25.719235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-04-12 11:50:25.727235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-04-12 11:50:25.731235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-04-12 11:50:25.735235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-04-12 11:50:25.739235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-04-12 11:50:25.743235 authentik_client-2024.2.2.post1712922614/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0     5545 2024-04-12 11:50:25.747235 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-04-12 11:50:25.751236 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-04-12 11:50:25.755236 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-04-12 11:50:25.755236 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-04-12 11:50:25.759236 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-04-12 11:50:25.763236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-04-12 11:50:25.767236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-04-12 11:50:25.771236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-04-12 11:50:25.775236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-04-12 11:50:25.779236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-04-12 11:50:25.783236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-04-12 11:50:25.783236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-04-12 11:50:25.787236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-04-12 11:50:25.791236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-04-12 11:50:25.795236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.799236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-04-12 11:50:25.799236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-04-12 11:50:25.803236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.807236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-12 11:50:25.811236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-04-12 11:50:25.811236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-04-12 11:50:25.815236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-04-12 11:50:25.819236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.823236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-12 11:50:25.823236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.827236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-04-12 11:50:25.831236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-04-12 11:50:25.835236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-04-12 11:50:25.835236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-04-12 11:50:25.839236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-04-12 11:50:25.843236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-04-12 11:50:25.847236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-04-12 11:50:25.847236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-12 11:50:25.851236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-04-12 11:50:25.855236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3274 2024-04-12 11:50:25.859236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-04-12 11:50:25.867236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-12 11:50:25.871236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-04-12 11:50:25.871236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-04-12 11:50:25.875236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-04-12 11:50:25.879236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-04-12 11:50:25.883236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.883236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.887236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-12 11:50:25.891236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3330 2024-04-12 11:50:25.895236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-04-12 11:50:25.895236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-04-12 11:50:25.899237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-04-12 11:50:25.903236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-04-12 11:50:25.907236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-04-12 11:50:25.907236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-12 11:50:25.911236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-04-12 11:50:25.915237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-04-12 11:50:25.919237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-04-12 11:50:25.923236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-12 11:50:25.927237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-04-12 11:50:25.931237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.935237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-04-12 11:50:25.939237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-04-12 11:50:25.943237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-04-12 11:50:25.943237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-04-12 11:50:25.947237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-04-12 11:50:25.951237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-04-12 11:50:25.955237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-12 11:50:25.959237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-04-12 11:50:25.963237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-12 11:50:25.967237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-04-12 11:50:25.971237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-04-12 11:50:25.971237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-04-12 11:50:25.975237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-04-12 11:50:25.979237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-04-12 11:50:25.979237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-04-12 11:50:25.983237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-12 11:50:25.987237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-04-12 11:50:25.987237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.991237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.995237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-12 11:50:25.995237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.999237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3331 2024-04-12 11:50:26.003237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-04-12 11:50:26.007237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-04-12 11:50:26.003237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-04-12 11:50:26.011237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-12 11:50:26.011237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-04-12 11:50:26.015237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-04-12 11:50:26.019237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-12 11:50:26.023237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-04-12 11:50:26.027237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-04-12 11:50:26.031237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-04-12 11:50:26.035237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-04-12 11:50:26.023237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-04-12 11:50:26.035237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-04-12 11:50:26.039237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-04-12 11:50:26.043237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-04-12 11:50:26.043237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-04-12 11:50:26.051237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-04-12 11:50:26.051237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-04-12 11:50:26.055237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-04-12 11:50:26.059237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-04-12 11:50:26.059237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-04-12 11:50:26.063237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-04-12 11:50:26.067237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-04-12 11:50:26.071237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-04-12 11:50:26.075237 authentik_client-2024.2.2.post1712922614/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-04-12 11:50:26.079237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-04-12 11:50:26.079237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-04-12 11:50:26.083237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-04-12 11:50:26.087237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-04-12 11:50:26.087237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-04-12 11:50:26.091237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-04-12 11:50:26.095237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-04-12 11:50:26.099238 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-12 11:50:26.099238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-04-12 11:50:26.103237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-04-12 11:50:26.107237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-04-12 11:50:26.111237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-04-12 11:50:26.111237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4931 2024-04-12 11:50:26.115238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-04-12 11:50:26.119238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-04-12 11:50:26.123237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-04-12 11:50:26.123237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-04-12 11:50:26.127238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-04-12 11:50:26.131238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-04-12 11:50:26.131238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-04-12 11:50:26.135238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-04-12 11:50:26.139238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-04-12 11:50:26.139238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-04-12 11:50:26.143238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-04-12 11:50:26.147238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-04-12 11:50:26.147238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-04-12 11:50:26.151238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-04-12 11:50:26.155238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-04-12 11:50:26.159238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-04-12 11:50:26.163238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-04-12 11:50:26.167238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-04-12 11:50:26.171238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-04-12 11:50:26.175238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-04-12 11:50:26.179238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3385 2024-04-12 11:50:26.183238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-04-12 11:50:26.187238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3985 2024-04-12 11:50:26.191238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-04-12 11:50:26.195238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-04-12 11:50:26.195238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-04-12 11:50:26.199238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-04-12 11:50:26.203238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-04-12 11:50:26.211238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-04-12 11:50:26.215238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2879 2024-04-12 11:50:26.219238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-04-12 11:50:26.223238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-04-12 11:50:26.223238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-04-12 11:50:26.227238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-04-12 11:50:26.231238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-04-12 11:50:26.231238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-04-12 11:50:26.235238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-04-12 11:50:26.239238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-04-12 11:50:26.243238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-04-12 11:50:26.243238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-04-12 11:50:26.247238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-04-12 11:50:26.251238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-04-12 11:50:26.255238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-04-12 11:50:26.263238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-04-12 11:50:26.267238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-04-12 11:50:26.267238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-04-12 11:50:26.271238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-04-12 11:50:26.275238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-04-12 11:50:26.275238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-04-12 11:50:26.279238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-04-12 11:50:26.283238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-04-12 11:50:26.283238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-04-12 11:50:26.287238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-04-12 11:50:26.291238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-04-12 11:50:26.291238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-04-12 11:50:26.295238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-04-12 11:50:26.299239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3819 2024-04-12 11:50:26.303238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     5079 2024-04-12 11:50:26.307238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-04-12 11:50:26.299239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-04-12 11:50:26.311239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-04-12 11:50:26.311239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-04-12 11:50:26.319239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4419 2024-04-12 11:50:26.323238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-04-12 11:50:26.315239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-04-12 11:50:26.327239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-04-12 11:50:26.331239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-04-12 11:50:26.339239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-04-12 11:50:26.339239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-04-12 11:50:26.347239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-04-12 11:50:26.351239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-04-12 11:50:26.355239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-04-12 11:50:26.355239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-04-12 11:50:26.359239 authentik_client-2024.2.2.post1712922614/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-04-12 11:50:26.359239 authentik_client-2024.2.2.post1712922614/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-04-12 11:50:26.363239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-04-12 11:50:26.367239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-04-12 11:50:26.371239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-04-12 11:50:26.371239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-04-12 11:50:26.375239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-04-12 11:50:26.379239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-04-12 11:50:26.379239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-04-12 11:50:26.383239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-04-12 11:50:26.387239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-04-12 11:50:26.387239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-04-12 11:50:26.391239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-04-12 11:50:26.391239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-04-12 11:50:26.395239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-04-12 11:50:26.395239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-04-12 11:50:26.399239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-04-12 11:50:26.403239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-04-12 11:50:26.407239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-04-12 11:50:26.407239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-04-12 11:50:26.411239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-04-12 11:50:26.415239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-04-12 11:50:26.415239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-04-12 11:50:26.419239 authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-04-12 11:50:26.419239 authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-04-12 11:50:26.423239 authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-04-12 11:50:26.427239 authentik_client-2024.2.2.post1712922614/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-04-12 11:50:26.427239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-04-12 11:50:26.431239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1314 2024-04-12 11:50:26.431239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-04-12 11:50:26.435239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-04-12 11:50:26.435239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-04-12 11:50:26.435239 authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-04-12 11:50:26.439239 authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-04-12 11:50:26.439239 authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-04-12 11:50:26.443239 authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-04-12 11:50:26.447239 authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-04-12 11:50:26.447239 authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-04-12 11:50:26.451239 authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-04-12 11:50:26.451239 authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-04-12 11:50:26.455239 authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-04-12 11:50:26.455239 authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-04-12 11:50:26.459239 authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-04-12 11:50:26.463239 authentik_client-2024.2.2.post1712922614/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-04-12 11:50:26.463239 authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-04-12 11:50:26.467239 authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-04-12 11:50:26.467239 authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-04-12 11:50:26.471239 authentik_client-2024.2.2.post1712922614/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-04-12 11:50:26.471239 authentik_client-2024.2.2.post1712922614/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-04-12 11:50:26.475239 authentik_client-2024.2.2.post1712922614/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-04-12 11:50:26.475239 authentik_client-2024.2.2.post1712922614/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-04-12 11:50:26.479239 authentik_client-2024.2.2.post1712922614/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-04-12 11:50:26.479239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-04-12 11:50:26.483240 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-04-12 11:50:26.483240 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-04-12 11:50:26.487239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-04-12 11:50:26.491239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-04-12 11:50:26.491239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-04-12 11:50:26.495239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-04-12 11:50:26.495239 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-04-12 11:50:26.499240 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-04-12 11:50:26.503239 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-04-12 11:50:26.503239 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     3131 2024-04-12 11:50:26.507239 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_sync_status.py
+-rw-r--r--   0        0        0     4629 2024-04-12 11:50:26.515240 authentik_client-2024.2.2.post1712922614/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-04-12 11:50:26.519240 authentik_client-2024.2.2.post1712922614/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-04-12 11:50:26.523240 authentik_client-2024.2.2.post1712922614/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-04-12 11:50:26.527240 authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-04-12 11:50:26.527240 authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-04-12 11:50:26.531240 authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-04-12 11:50:26.535240 authentik_client-2024.2.2.post1712922614/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4931 2024-04-12 11:50:26.539240 authentik_client-2024.2.2.post1712922614/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     5058 2024-04-12 11:50:26.539240 authentik_client-2024.2.2.post1712922614/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-04-12 11:50:26.543240 authentik_client-2024.2.2.post1712922614/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-04-12 11:50:26.543240 authentik_client-2024.2.2.post1712922614/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     1492 2024-04-12 11:50:26.543240 authentik_client-2024.2.2.post1712922614/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-04-12 11:50:26.511240 authentik_client-2024.2.2.post1712922614/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-04-12 11:50:26.515240 authentik_client-2024.2.2.post1712922614/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-04-12 11:50:26.547240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-04-12 11:50:26.551240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-04-12 11:50:26.551240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-04-12 11:50:26.555240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-04-12 11:50:26.555240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-04-12 11:50:26.559240 authentik_client-2024.2.2.post1712922614/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-04-12 11:50:26.559240 authentik_client-2024.2.2.post1712922614/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-04-12 11:50:26.563240 authentik_client-2024.2.2.post1712922614/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-04-12 11:50:26.563240 authentik_client-2024.2.2.post1712922614/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-04-12 11:50:26.567240 authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-04-12 11:50:26.567240 authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-04-12 11:50:26.571240 authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-04-12 11:50:26.571240 authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-04-12 11:50:26.575240 authentik_client-2024.2.2.post1712922614/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     4463 2024-04-12 11:50:26.575240 authentik_client-2024.2.2.post1712922614/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-04-12 11:50:26.575240 authentik_client-2024.2.2.post1712922614/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4286 2024-04-12 11:50:26.579240 authentik_client-2024.2.2.post1712922614/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-04-12 11:50:26.579240 authentik_client-2024.2.2.post1712922614/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-04-12 11:50:26.587240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-04-12 11:50:26.591240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-04-12 11:50:26.591240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-04-12 11:50:26.595240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-04-12 11:50:26.595240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4802 2024-04-12 11:50:26.599240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token.py
+-rw-r--r--   0        0        0     4198 2024-04-12 11:50:26.603240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4329 2024-04-12 11:50:26.607240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-04-12 11:50:26.607240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-04-12 11:50:26.611240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-04-12 11:50:26.583240 authentik_client-2024.2.2.post1712922614/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-04-12 11:50:26.583240 authentik_client-2024.2.2.post1712922614/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-04-12 11:50:26.615240 authentik_client-2024.2.2.post1712922614/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-04-12 11:50:26.619240 authentik_client-2024.2.2.post1712922614/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-04-12 11:50:26.619240 authentik_client-2024.2.2.post1712922614/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-04-12 11:50:26.623240 authentik_client-2024.2.2.post1712922614/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-04-12 11:50:26.623240 authentik_client-2024.2.2.post1712922614/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-04-12 11:50:26.627240 authentik_client-2024.2.2.post1712922614/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5226 2024-04-12 11:50:26.627240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-04-12 11:50:26.631240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-04-12 11:50:26.635240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3828 2024-04-12 11:50:26.635240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-04-12 11:50:26.639240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-04-12 11:50:26.639240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-12 11:50:26.643240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-04-12 11:50:26.647240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-04-12 11:50:26.647240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     3193 2024-04-12 11:50:26.651240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_group_request.py
+-rw-r--r--   0        0        0     4334 2024-04-12 11:50:26.655240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-04-12 11:50:26.659240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-04-12 11:50:26.659240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-04-12 11:50:26.663240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-04-12 11:50:26.663240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-12 11:50:26.667240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-04-12 11:50:26.667240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-04-12 11:50:26.671240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-04-12 11:50:26.675240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-04-12 11:50:26.675240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-04-12 11:50:26.679240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-04-12 11:50:26.683241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-04-12 11:50:26.683241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-04-12 11:50:26.687240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-04-12 11:50:26.687240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-04-12 11:50:26.691240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-04-12 11:50:26.695240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-04-12 11:50:26.699241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-04-12 11:50:26.699241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-04-12 11:50:26.703240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-04-12 11:50:26.703240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-04-12 11:50:26.707240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-04-12 11:50:26.707240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-04-12 11:50:26.711241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-04-12 11:50:26.715241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-04-12 11:50:26.715241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-04-12 11:50:26.719241 authentik_client-2024.2.2.post1712922614/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-04-12 11:50:26.723241 authentik_client-2024.2.2.post1712922614/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3630 2024-04-12 11:50:26.727241 authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-04-12 11:50:26.727241 authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-04-12 11:50:26.731241 authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-04-12 11:50:26.735241 authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-04-12 11:50:26.735241 authentik_client-2024.2.2.post1712922614/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:50:27.899247 authentik_client-2024.2.2.post1712922614/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-04-12 11:50:27.911247 authentik_client-2024.2.2.post1712922614/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-04-12 11:50:27.899247 authentik_client-2024.2.2.post1712922614/pyproject.toml
+-rw-r--r--   0        0        0   141408 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1712922614/PKG-INFO
```

### Comparing `authentik_client-2024.2.2.post1712833897/README.md` & `authentik_client-2024.2.2.post1712922614/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1712833897
+- Package version: 2024.2.2-1712922614
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -62,19 +62,18 @@
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
-# Configure API key authorization: authentik
-configuration.api_key['authentik'] = os.environ["API_KEY"]
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['authentik'] = 'Bearer'
+# Configure Bearer authorization: authentik
+configuration = authentik_client.Configuration(
+    access_token = os.environ["BEARER_TOKEN"]
+)
 
 
 # Enter a context with an instance of the API client
 with authentik_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = authentik_client.AdminApi(api_client)
 
@@ -1375,17 +1374,15 @@
 ## Documentation For Authorization
 
 
 Authentication schemes defined for the API:
 <a id="authentik"></a>
 ### authentik
 
-- **Type**: API key
-- **API key parameter name**: Authorization
-- **Location**: HTTP header
+- **Type**: Bearer authentication
 
 
 ## Author
 
 hello@goauthentik.io
```

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/__init__.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.2.2-1712833897"
+__version__ = "2024.2.2-1712922614"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
```

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/__init__.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/admin_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/authenticators_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/authenticators_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/core_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/crypto_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/crypto_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/enterprise_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/enterprise_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/events_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/flows_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/flows_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/managed_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/managed_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/oauth2_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/oauth2_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/outposts_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/outposts_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/policies_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/propertymappings_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/providers_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/providers_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/rac_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/rac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/rbac_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/rbac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/root_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/root_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/schema_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/sources_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/stages_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/stages_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api/tenants_api.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api_client.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.2.2-1712833897/python'
+        self.user_agent = 'OpenAPI-Generator/2024.2.2-1712922614/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/api_response.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/configuration.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,33 +53,14 @@
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum
       values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
       in PEM format.
 
     :Example:
-
-    API Key Authentication Example.
-    Given the following security scheme in the OpenAPI specification:
-      components:
-        securitySchemes:
-          cookieAuth:         # name for the security scheme
-            type: apiKey
-            in: cookie
-            name: JSESSIONID  # cookie name
-
-    You can programmatically set the cookie:
-
-conf = authentik_client.Configuration(
-    api_key={'cookieAuth': 'abc123'}
-    api_key_prefix={'cookieAuth': 'JSESSIONID'}
-)
-
-    The following cookie will be added to the HTTP request:
-       Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
@@ -376,35 +357,33 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
-        if 'authentik' in self.api_key:
+        if self.access_token is not None:
             auth['authentik'] = {
-                'type': 'api_key',
+                'type': 'bearer',
                 'in': 'header',
                 'key': 'Authorization',
-                'value': self.get_api_key_with_prefix(
-                    'authentik',
-                ),
+                'value': 'Bearer ' + self.access_token
             }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2024.2.2\n"\
-               "SDK Package Version: 2024.2.2-1712833897".\
+               "SDK Package Version: 2024.2.2-1712922614".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/exceptions.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/__init__.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/access_denied_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/app.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/app.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/app_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/app_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/apple_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/apple_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/application.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/application.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/application_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/auth_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/auth_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_asn.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authentication_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authentication_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_attachment_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validate_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validation_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/autosubmit_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/backends_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/backends_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/binding_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/blueprint_file.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_file.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/brand.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/brand_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/cache.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/cache.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/capabilities_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/captcha_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/certificate_data.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_data.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_generation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_key_pair.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/challenge_choices.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/challenge_choices.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/challenge_types.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/client_type_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/client_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/config.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/connection_token.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/connection_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/connection_token_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_permission.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/contextual_flow_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/coordinate.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/current_brand.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/current_brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/denied_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/deny_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/deny_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/device.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/device_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/device_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/device_challenge_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/device_classes_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/digest_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/digits_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/digits_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/docker_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/domain.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/domain.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/domain_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_policy.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/duo_device.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device_enrollment_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/duo_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_response_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/email_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/email_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/email_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/email_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/email_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/email_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/endpoint.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/endpoint_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/error_detail.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/error_reporting_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/event.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/event_actions.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_actions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_matcher_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/event_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_top_per_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/expiring_base_grant_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/expression_policy.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/expression_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/extra_role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/extra_user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/file_path_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/file_path_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_designation_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_diagram.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_diagram.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_error_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_import_result.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_import_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_inspection.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_inspection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_inspector_plan.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_set.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_set.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_set_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_stage_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/footer_link.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/footer_link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/generic_error.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/generic_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/geoip_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/group.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/group_member.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/group_member_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/group_member_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/group_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/identification_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/identification_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/install_id.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/install_id.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/intent_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/intent_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/invalid_response_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/invitation.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/invitation_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/invitation_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/issuer_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/kubernetes_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_debug.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_debug.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_provider.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_source.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldap_sync_status.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldapapi_access_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/license.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/license.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/license_forecast.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/license_forecast.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/license_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/license_summary.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/license_summary.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/link.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/log_event.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/log_event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/log_level_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/log_level_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/login_challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/login_metrics.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/login_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/login_source.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/login_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/metadata.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/model_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/model_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/model_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/name_id_policy_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/network_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/not_configured_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_rule.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_rule.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_transport.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_test.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_webhook_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_source.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/open_id_connect_configuration.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_default_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost_health.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_health.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_brand_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_connection_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_consent_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_deny_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_domain_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_duo_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_email_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_event_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_expression_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_flow_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_identification_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_invitation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_license_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_rule_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_transport_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_outpost_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_plex_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_prompt_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_rac_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_radius_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_reputation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scim_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_sms_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_source_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_static_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_system_task_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_tenant_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_token_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_totp_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_consent_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/pagination.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/password_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_expiry_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/password_policy.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/password_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/password_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/password_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_application_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_event_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_group_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_license_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_role_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_token_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/permission.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_authentication_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_source.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_token_redeem_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/policy.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_binding.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_engine_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_test_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_test_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/policy_test_result.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/property_mapping.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping_preview.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/protocol_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/protocol_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/provider.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/provider_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/proxy_mode.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/proxy_provider.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/rac_provider.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/radius_provider.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/redirect_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/reputation.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/reputation_policy.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/resident_key_requirement_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/role.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/role.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/role_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/role_object_permission.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/role_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_metadata.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_provider.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_source.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/saml_source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_mapping.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_provider.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/scim_sync_status.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/scope_mapping.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/scope_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/selectable_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/selectable_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/service_connection.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/service_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/service_connection_state.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection_state.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/session_user.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/session_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/settings.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/settings.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/settings_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/severity_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/severity_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/shell_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/shell_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/signature_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/sms_device.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/sms_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/sms_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/source.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/source_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/source_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/source_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/source_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/source_type.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/sp_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/stage_prompt.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/stage_prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/static_device.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/static_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/static_device_token.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/sub_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/system_info.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/system_info_runtime.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/system_task.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/system_task.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/system_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_recovery_key_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/tenant_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/token.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/token_model.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/token_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/token_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/token_set_key_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/token_view.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/token_view.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/totp_device.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/totp_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/totp_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/transaction_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/transaction_application_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/type_create.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/type_create.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/ui_theme_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/used_by.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/used_by.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/used_by_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_account_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_consent.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_consent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_creation_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_delete_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_fields_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_group.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_group_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_login_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_logout_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_matching_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_metrics.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_o_auth_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_object_permission.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_password_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_path.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_path.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_saml_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_self.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_self.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_self_groups.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_self_groups.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_service_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_service_account_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_setting.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_setting.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_source_connection.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_type_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_verification_enum.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_verification_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_write_stage.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_write_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/validation_error.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/version.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/version.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/web_authn_device.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/web_authn_device_type.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/web_authn_device_type_request.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_type_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/models/workers.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/models/workers.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/authentik_client/rest.py` & `authentik_client-2024.2.2.post1712922614/authentik_client/rest.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712833897/pyproject.toml` & `authentik_client-2024.2.2.post1712922614/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.2.2-1712833897"
+version = "2024.2.2-1712922614"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.2.2.post1712833897/PKG-INFO` & `authentik_client-2024.2.2.post1712922614/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.2.2.post1712833897
+Version: 2024.2.2.post1712922614
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -25,15 +25,15 @@
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1712833897
+- Package version: 2024.2.2-1712922614
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -87,19 +87,18 @@
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
-# Configure API key authorization: authentik
-configuration.api_key['authentik'] = os.environ["API_KEY"]
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['authentik'] = 'Bearer'
+# Configure Bearer authorization: authentik
+configuration = authentik_client.Configuration(
+    access_token = os.environ["BEARER_TOKEN"]
+)
 
 
 # Enter a context with an instance of the API client
 with authentik_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = authentik_client.AdminApi(api_client)
 
@@ -1400,17 +1399,15 @@
 ## Documentation For Authorization
 
 
 Authentication schemes defined for the API:
 <a id="authentik"></a>
 ### authentik
 
-- **Type**: API key
-- **API key parameter name**: Authorization
-- **Location**: HTTP header
+- **Type**: Bearer authentication
 
 
 ## Author
 
 hello@goauthentik.io
```

