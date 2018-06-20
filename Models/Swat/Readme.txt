--material--
    object->SetMaterial(0, cache->GetResource<Material>("Models/Swat/Materials/Soldier_body1.xml") );
    object->SetMaterial(1, cache->GetResource<Material>("Models/Swat/Materials/Soldier_head6.xml") );
    object->SetMaterial(2, cache->GetResource<Material>("Models/Swat/Materials/Soldier_body1.xml") );

--capsule setting--
    // Set a capsule shape for collision
    CollisionShape* shape = objectNode->CreateComponent<CollisionShape>();
    shape->SetCapsule(0.7f, 1.8f, Vector3(0.0f, 0.94f, 0.0f));

--velocities--
Based on the animation duration and the distance traveled:
    walk - 1.842 m/s
    run - 4.78 m/s
    sprint - 7.164 m/s
