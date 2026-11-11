ALL MOTIVE DEALERS — WEBSITE UPDATE FILES

Included:
- config.js: Supabase project URL and publishable browser key.
- admin/index.html: private manager login and vehicle dashboard.

Your original public index.html and assets folder are not replaced by this package.

TO ADD TO GITHUB:
1. Open your repository: https://github.com/pmumo762-stack/allmotivedealers.github.io
2. Upload config.js into the repository root.
3. Create folder admin and upload admin/index.html into it.
4. The manager page will be at https://pmumo762-stack.github.io/allmotivedealers.github.io/admin/

IMPORTANT:
This creates the admin page files only. The public index.html still needs a small code change to fetch vehicle records from Supabase instead of its existing hard-coded array. Do not delete your assets folder. Existing Supabase RLS policies must enforce manager-only insert/update/delete; the email check in this page is not a security boundary. The storage bucket must allow public image reads and manager-only uploads/updates/deletes.

The admin uses:
- Supabase table: vehicles
- Storage bucket: vehicle-photos
- Manager email: pmumo762@gmail.com

Do not add any service-role or secret key to website files.
