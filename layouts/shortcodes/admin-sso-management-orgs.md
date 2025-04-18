{{ $product_link := "[Docker Hub](https://hub.docker.com)" }}
{{ $sso_navigation := "Select **My Hub**, your organization, and then **Settings**." }}
{{ if eq (.Get "product") "admin" }}
  {{ $product_link = "the [Admin Console](https://app.docker.com/admin)" }}
  {{ $sso_navigation = "Select your company from the **Choose profile** page, and then select **SSO and SCIM**." }}
{{ end }}

### Connect an organization

1. Sign in to {{ $product_link }}.
2. {{ $sso_navigation }}
3. In the SSO connections table, select the **Action** icon and then **Edit connection**.
4. Select **Next** to navigate to the section where connected organizations are listed.
5. In the **Organizations** drop-down, select the organization to add to the connection.
6. Select **Next** to confirm or change the default organization and team provisioning.
7. Review the **Connection Summary** and select **Update connection**.

### Remove an organization

1. Sign in to {{ $product_link }}.
2. {{ $sso_navigation }}
3. In the SSO connections table, select the **Action** icon and then **Edit connection**.
4. Select **Next** to navigate to the section where connected organizations are listed.
5. In the **Organizations** drop-down, select **Remove** to remove the connection.
6. Select **Next** to confirm or change the default organization and team provisioning.
7. Review the **Connection Summary** and select **Update connection**.
